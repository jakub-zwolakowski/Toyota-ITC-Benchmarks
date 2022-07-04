# Tests

1. bit_shift: FLAWLESS
2. buffer_overrun_dynamic: FLAWLESS
3. buffer_underrun_dynamic
   - UB-039(137) - false negative - FAULTY TEST
   - OK-037(174) - false positive - FAULTY TEST
4. cmp_funcadr
   - UB-001(177) - false negative - NOT UB
   - UB-002(178) - false negative - NOT UB
5. conflicting_cond
   - all UB tests (181-190): false negative - NOT UB, DEAD CODE CORRECTLY DETECTED
6. data_lost
   - UB-010(210): false negative
   - UB-012(212): false negative
   - OK-006(225): false positive
7. data_overflow
   - UB-009(247)
   - UB-010(248)
   - OK-007(270)
   - OK-008(271)
   - OK-024(287)
   - OK-025(289)
8. data_underflow
   - UB-007(295)
   - UB-008(296)
   - UB-012(300)
9. dead_code
   - all UB: false negative
10. dead_lock
    - all UB : false negative
11. deletion_of_data_structure_sentinel
    - all UB : false negative
12. double_free: FLAWLESS
13. double_lock
    - all UB : false negative
14. double_release
    - almost all UB : false negative
15. endless_loop: FLAWLESS WHEN CORRECTED!
16. free_nondynamic_allocated_memory: FLAWLESS
17. free_null_pointer
    - UB-001(449)
    - UB-002(450)
    - UB-003(451)
    - UB-004(452)
    - UB-007(455)
18. func_pointer: FLAWLESS
19. function_return_value_unchecked
    - all UB : false negative
20. improper_termination_of_block
    - all UB : false negative
    - UB-004(542) : OOM
21. insign_code
    - all UB : false negative
22. invalid_extern
    - TODO
23. invalid_memory_access
    - UB-003(563)
    - UB-014(574)
    - UB-015(575)
24. littlemem_st
    - OK-008(613)
    - OK-009(614)
    - OK-010(615)
    - OK-011(616)
25. livelock
    - UB-001(617)
26. lock_never_unlock
    - all UB : false negative
    - also: function `sleep` is not defined
27. memory_allocation_failure
    - UB-001(637): OOM
    - UB-005(641)
    - UB-006(642)
    - UB-009(645): OOM
    - UB-010(646): OOM
    - UB-014(650)
28. memory_leak
    - UB-001(669): Timeout
    - all UB: false negative
29. not_return
    - UB-002(706)
    - UB-003(707)
    - UB-004(708)
30. null_pointer
    - UB-016(728)
31. overrun_st
    - OK-001(801)
    - OK-002(802)
    - OK-006(806)
    - OK-007(807)
    - OK-022(822)
    - OK-023(823)
    - OK-027(827)
    - OK-028(828)
    - OK-053(853)
32. ow_memcpy
    - UB-001(855)
    - UB-002(856)
33. pow_related_errors
    - all UB : false negative
34. ptr_subtraction
    - UB-001(917)
    - OK-001(919)
35. race_condition
    - all UB: false negative
36. redundant_cond
    - all UB: false negative
37. return_local: FLAWLESS
38. sign_conv
    - UB-009(977)
39. sleep_lock
    - all UB: false negative
40. st_cross_thread_access
    - all UB: false negative
41. st_overflow
    - UB-001(1025)
    - UB-002(1026)
    - UB-003(1027)
    - UB-004(1028)
    - UB-005(1029)
    - UB-007(1031)
    - OK-006(1037)
42. st_underrun
    - OK-002(1047)
    - OK-007(1052)
43. underrun_st
    - OK-008(1073)
    - OK-010(1075)
    - OK-012(1077)
44. uninit_memory_access
    - UB-002(1080)
    - UB-004(1082)
    - UB-005(1083)
    - UB-012(1090)
    - UB-013(1091)
45. uninit_pointer
    - UB-004(1112)
    - UB-008(1116)
    - UB-010(1118)
    - UB-013(1121)
    - UB-014(1122)
    - OK-012(1136)
46. uninit_var
    - UB-001(1141)
    - ...
    - UB-008(1148)
    - UB-010(1150)
    - UB-015(1155)
47. unlock_without_lock
    - all UB: false negative
48. unused_var
    - all UB: false negative
49. wrong_arguments_func_pointer
    - UB-018(1218)
    - OK-014(1232)
50. zero_division
    - UB-008(1244)
    - UB-010(1246)
