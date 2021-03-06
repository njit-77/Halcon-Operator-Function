# HALCON 算子函数

## Chapter 2 : Develop(外部函数)

| 序号 | 函数名                      | 函数说明及注释                                               | 页码 |
| ---- | --------------------------- | ------------------------------------------------------------ | ---- |
| 1    | dev_clear_obj               | 从Halcon数据库中删除一个不需要的图标物体                     | 23   |
| 2    | dev_clear_window            | 清除活动图形窗口的图形                                       | 24   |
| 3    | dev_close_inspect_ctrl      | 关闭一个控制变量的检查/测量窗口                              | 24   |
| 4    | dev_close_window            | 关闭活动图形窗口                                             | 24   |
| 5    | dev_display                 | 在现有图形窗口中显示图像目标                                 | 24   |
| 6    | dev_error_var               | 定义一个错误变量，并设置是否打开该错误状态                   | 24   |
| 7    | dev_get_exception_data      | 存取一个数组的元素                                           | 24   |
| 8    | dev_get_preferences         | 通过设计查询HDevelop的参数选择                               | 24   |
| 9    | dev_inspect_ctrl            | 打开一个或多个控制变量的监视窗口                             | 24   |
| 10   | dev_map_par                 | 打开一个可视化对话框来设置参数，相当于打开菜单/可视化/设置参数 | 24   |
| 11   | dev_map_prog                | 是HDevelop的主窗口可视化                                     | 24   |
| 12   | dev_map_var                 | 在屏幕上打开一个变量窗口                                     | 25   |
| 13   | dev_open_window             | 打开一个图形窗口                                             | 25   |
| 14   | dev_set_check               | 指定错误检查，检测错误状态是否为 2(H_MSG_TRUE)               | 25   |
| 15   | dev_set_color               | 设置一个颜色用在某个显示region（区域），图形或XLD            | 25   |
| 16   | dev_set_colored             | 设置混合颜色用在某个显示region（区域），图形或XLD            | 25   |
| 17   | dev_set_draw                | 定义区域填充模式                                             | 25   |
| 18   | dev_set_line_width          | 定义区域轮廓输出的线宽                                       | 25   |
| 19   | dev_set_lut                 | 设置颜色查询表                                               | 25   |
| 20   | dev_set_paint               | 定义灰度值输出模式                                           | 25   |
| 21   | dev_set_part                | 在当前窗口显示设定区域大小的图像                             | 26   |
| 22   | dev_set_preferences         | 通过设计设置HDevelop的参数选择                               | 26   |
| 23   | dev_set_shape               | 定于区域输出形状（原始、图形、随意圆、小圆、矩形、椭圆、图标等） | 26   |
| 24   | dev_set_window              | 激活一个图形窗口                                             | 26   |
| 25   | dev_set_window_externs      | 改变一个图形窗口的大小及位置                                 | 26   |
| 26   | dev_unmap_par               | 关闭一个可视化对话框来设置参数                               | 26   |
| 27   | dev_unmap_prog              | 关闭一个Halcon主窗口，关闭一个Halcon软件                     | 26   |
| 28   | dev_unmap_var               | 在屏幕上关闭一个变量窗口                                     | 26   |
| 29   | dev_update_pc               | 在程序执行中指定PC的行为，更新程序计数器                     | 26   |
| 30   | dev_update_time             | 为操作符打开或关闭切换时间测量，显示处理时间                 | 27   |
| 31   | dev_update_var              | 在程序执行中指定活动窗口的行为，更新变量                     | 27   |
| 32   | dev_update_window           | 在程序执行中指定输出行为，更新图像窗口                       | 27   |
| 33   | dev_open_window_fit_image   | 按指定图像的大小来打开一个窗口                               | 27   |
| 34   | dev_open_window_fit_size    | 按指定图像的尺寸开打开一个窗口                               | 27   |
| 35   | dev_resize_window_fit_image | 按图像的大小刷新一个窗口                                     | 28   |
| 36   | dev_resize_window_fit_size  | 按给定的尺寸来刷新一个窗口大小                               | 28   |
| 37   | dev_update_off              | 关闭dev_update_pc/_var/dev_update_window,停止刷新pc/变量/窗口 | 28   |
| 38   | dev_update_on               | 打开dev_update_pc/_var/dev_update_window,停止刷新pc/变量/窗口 | 28   |

## Chapter 3 : Measuring-1D(1D测量)

### 3.1 Measuring-1D高斯混合模型

| 序号 | 函数名                      | 函数说明及注释                                               | 页码 |
| ---- | --------------------------- | ------------------------------------------------------------ | ---- |
| 1    | close_all_measures          | 清除所有测量对象                                             | 31   |
| 2    | close_measure               | 清除一个测量对象                                             | 31   |
| 3    | fuzzy_meausre_pairing       | 模糊测量配对，提取与矩形或环状弧垂直的直线边缘的起点、终点、中间点的坐标值，并提供起点和终点两点之间的间距 | 31   |
| 4    | fuzzy_measure_pairs         | 模糊测量配对，提取与矩形或环状弧垂直的直线边缘的起点、终点、中间点的坐标值，并提供起点和终点两点之间的间距，终点至下一配对起点的间距 | 32   |
| 5    | fuzzy_measure_pos           | 模糊测量配对，提取与矩形或环状弧垂直的直线边缘，提供匹配边缘的中点坐标值，并提供该点至下一匹配点的间距 | 32   |
| 6    | gen_measure_arc             | 提取与圆弧垂直中心轴线的直线边沿，设定ROI                    | 33   |
| 7    | gen_measure_rectangle2      | 提取与矩形垂直中心轴线的直线边沿，设定ROI                    | 33   |
| 8    | measure_pairs               | 提取与矩形或环状弧垂直的直线边缘的起点、终点、中间点的坐标值，并提供起点和终点两点之间的间距，终点至下一配对起点的间距 | 36   |
| 9    | measure_pos                 | 提取与矩形或环状弧垂直的直线边缘，提供匹配边缘的中点坐标值，并提供该点至下一匹配点的间距 | 37   |
| 10   | measure_projection          | 提取垂直与一个矩形或环状弧的灰度值轮廓(contour)              | 38   |
| 11   | measure_thresh              | 提取沿着一个矩形或环状弧，特殊灰度值的点                     | 38   |
| 12   | reset_fuzzy_measure         | 重置一个模糊元函数                                           | 38   |
| 13   | set_fuzzy_measure           | 指定一个模糊元函数                                           | 38   |
| 14   | set_fuzzy_measure_norm_pair | 为边缘匹配指定一个规范画模糊元函数                           | 38   |
| 15   | translate_measure           | 转化（解释）一个测试对象                                     | 39   |

## Chapter 4: Matching-3D(3D匹配)

### 4.1 Shape-Based外形匹配

| 序号 | 函数名                        | 函数说明及注释                                               | 页码 |
| ---- | ----------------------------- | ------------------------------------------------------------ | ---- |
| 1    | clear_all_shape_model_3d      | 清除所有3D轮廓模型，释放内存空间                             | 45   |
| 2    | clear_shape_model_3d          | 清除指定3D轮廓模型，释放内存空间                             | 45   |
| 3    | create_cam_pose_look_at_point | 创建一个3D摄像机位置（从摄像机中心观察方向）                 | 45   |
| 4    | create_shape_model_3d         | 创建一个3D目标模型                                           | 45   |
| 5    | find_shape_model_3d           | 从图像中找出一个3D模型的最佳匹配                             | 46   |
| 6    | get_shape_model_3d_contours   | 提取3D轮廓目标                                               | 46   |
| 7    | get_shape_model_3d_params     | 提取一个3D轮廓模型的参数                                     | 46   |
| 8    | project_shape_model_3d        | 把一个3D轮廓模型的边缘投影到图像坐标中                       | 47   |
| 9    | read_shape_model_3d           | 读取一个3D轮廓模型文件                                       | 47   |
| 10   | trans_pose_shape_model_3d     | 把一个3D目标模型的坐标系中的位置转变为一个3D轮廓模型的参考坐标系中的位置，反之亦然 | 47   |
| 11   | write_shape_model_3d          | 把一个3D轮廓模型保存到文件中                                 | 47   |

### 4.2 Shrface-Based曲面匹配

| 序号 | 函数名                             | 函数说明及注释                       | 页码 |
| ---- | ---------------------------------- | ------------------------------------ | ---- |
| 1    | clear_all_surface_matching_results | 清除所有的曲面匹配目标，释放内存空间 | 48   |
| 2    | clear_all_surface_models           | 清除所有的曲面匹配模型，释放内存空间 | 48   |
| 3    | clear_surface_matching_result      | 清除指定的曲面匹配目标，释放内存空间 | 48   |
| 4    | clear_surface_model                | 清除指定的曲面匹配模型，释放内存空间 | 48   |
| 5    | create_surface_model               | 创建一个曲面匹配模型                 | 48   |
| 6    | find_surface_model                 | 从3D背景中找出最佳匹配               | 48   |
| 7    | get_surface_matching_result        | 提取曲面匹配目标                     | 49   |
| 8    | get_surface_model_param            | 提取曲面匹配模型参数                 | 49   |
| 9    | read_surface_model                 | 读取曲面匹配模型文件                 | 49   |
| 10   | refine_surface_model_pose          | 使3D背景中曲面模型坐标完善           | 49   |
| 11   | write_surface_model                | 将一个曲面匹配模型保存到文件中       | 49   |

## Chapter 5: Reconstruction-3D(3D复原)

### 5.1 Binocular Stereo 双目

| 序号 | 函数名                            | 函数说明及注释                                               | 页码 |
| ---- | --------------------------------- | ------------------------------------------------------------ | ---- |
| 1    | binocular_disparity               | 通过相互关系来计算两个图像的双目视觉差                       | 53   |
| 2    | binocular_disparity_mg            | 通过多格子方法来计算两个图像的双目视觉差                     | 54   |
| 3    | binocular_distance                | 通过相互关系来计算两个立体图像的双目视觉差                   | 54   |
| 4    | binocular_distance_mg             | 通过多格子方法来计算两个立体图像的双目视觉差                 | 54   |
| 5    | disparity_image_to_xyz            | 把一个观影距离转变成一个被矫正的3D立体点                     | 55   |
| 6    | disparity_to_distance             | 将观影距离转换为矫正双目视觉立体系统中的间隔值               | 55   |
| 7    | disparity_to_point_3d             | 将一个图像点和它的观影距离转换为一个矫正立体系统中的三维点   | 55   |
| 8    | distance_to_disparity             | 将一个间隔值转换为一个矫正立体系统中的观影距离               | 56   |
| 9    | essential_to_fundamental_matrix   | 计算一个从原始矩阵衍生而来的基础矩阵                         | 56   |
| 10   | gen_binocular_proj_rectification  | 计算双目视觉立体系统图像的投射矫正值                         | 56   |
| 11   | gen_binocular_rectification_map   | 创建转换图，其描述从一个双目相机到一个普通的矫正图像面的图像映射 | 56   |
| 12   | intersect_lines_of_sight          | 从一个双目相机系统视觉中两条线的交点中获取一个三维点         | 57   |
| 13   | match_essential_matrix_ransack    | 通过自动发掘图像点间对应关系来计算立体图像对应的原始（本质）矩阵 | 57   |
| 14   | match_fundamental_matrix_ransack  | 通过自动发掘图像点间对应关系来计算立体图像对应的基本矩阵     | 58   |
| 15   | match_rel_pose_ransack            | 通过自动发掘图像点间对应关系来计算两个相机间的相对方位       | 58   |
| 16   | reconst3d_from_fundamental_matrix | 计算基于基本矩阵点投影的三位重建                             | 59   |
| 17   | rel_pose_to_fundamental_matrix    | 计算两个相机相关方向中获取的基本矩阵                         | 60   |
| 18   | vector_to_essential_matrix        | 计算给定图像点间映射和已知相机矩阵的原始矩阵，重建三维点     | 60   |
| 19   | vector_to_fundamental_matrix      | 计算给定图像点间映射的集合的基本矩阵，重建三维点             | 60   |
| 20   | vector_to_rel_pose                | 计算给定图像点对应关系和已知相机参数的两相机间相对方位，重建三维点 | 61   |

### 5.2 Depth From Focus 焦点深度

| 序号 | 函数名                          | 函数说明及注释                         | 页码 |
| ---- | ------------------------------- | -------------------------------------- | ---- |
| 1    | depth_from_focus                | 利用多倍聚集灰度级提取高度（厚度）     | 62   |
| 2    | select_grayvalues_from_channels | 利用索引图像选择一个多通道图像的灰度值 | 62   |

### 5.3 Multi-View Stereo 多视角立体模型

| 序号 | 函数名                       | 函数说明及注释                         | 页码 |
| ---- | ---------------------------- | -------------------------------------- | ---- |
| 1    | clear_all_stereo_models      | 清除所有的多视角立体模型，释放内存空间 | 62   |
| 2    | clear_stereo_model           | 清除指定的多视角立体模型，释放内存空间 | 62   |
| 3    | create_stereo_model          | 创建一个多视角立体模型                 | 62   |
| 4    | get_stereo_model_image_pairs | 获取立体模型中双目（成对）图像的列表   | 62   |
| 5    | get_stereo_model_object      | 获取立体重建的中间结果（图标）         | 63   |
| 6    | get_stereo_model_param       | 提取多视角立体模型参数                 | 63   |
| 7    | reconstruct_points_stereo    | 重建多视角立体3D参考点                 | 63   |
| 8    | reconstruct_surface_stereo   | 重建多视角3D曲面                       | 63   |
| 9    | set_stereo_model_image_pairs | 指定双目（成对）图像的表面立体重建     | 63   |
| 10   | set_stereo_model_param       | 设置多视角立体模型参数                 | 64   |

### 5.4 Photometric Stereo 估测光源

| 序号 | 函数名             | 函数说明及注释                         | 页码 |
| ---- | ------------------ | -------------------------------------- | ---- |
| 1    | estimate_al_am     | 估测一个平面的反射率和反射光的数目     | 64   |
| 2    | estimate_sl_al_lr  | 估测一个光源的倾斜度和一个平面的反射率 | 64   |
| 3    | estimate_sl_al_zc  | 估测一个光源的倾斜度和一个平面的反射率 | 64   |
| 4    | estimate_tilt_lr   | 估测一个光源的倾斜                     | 65   |
| 5    | estimate_tilt_zc   | 估测一个光源的倾斜                     | 65   |
| 6    | phot_stereo        | 根据至少三个灰度值的图像来重建一个平面 | 65   |
| 7    | sfs_mod_lr         | 从一个灰度值图像重建一个平面           | 65   |
| 8    | sfs_orig_lr        | 从一个灰度值图像重建一个平面           | 66   |
| 9    | sfs_pentland       | 从一个灰度值图像重建一个平面           | 66   |
| 10   | shade_height_field | 重建一个表面灰色突起的图像             | 66   |

### 5.5 Sheet of Light 片光

| 序号 | 函数名                                    | 函数说明及注释                               | 页码 |
| ---- | ----------------------------------------- | -------------------------------------------- | ---- |
| 1    | apply_sheet_of_light_calibration          | 应用校准变换到不一致的图像                   | 67   |
| 2    | clear_all_sheet_of_light_models           | 清除所有的片光模型，释放内存空间             | 67   |
| 3    | clear_sheet_of_light_model                | 清除指定片光模型，释放内存空间               | 67   |
| 4    | create_sheet_of_light_model               | 创建一个基于3D测量的片光模型                 | 67   |
| 5    | get_sheet_of_light_param                  | 提取片光模型的参数                           | 68   |
| 6    | get_sheet_of_light_result                 | 提取一个通过片光技术获得的测量结果（图标）   | 68   |
| 7    | get_sheet_of_light_result_object_model_3d | 提取一个通过片光技术获得的3D对象模型测量结果 | 68   |
| 8    | measure_profile_sheet_of_light            | 对输入和存储的轮廓图像记性片光技术处理       | 68   |
| 9    | query_sheet_of_light_params               | 提取参数列表                                 | 68   |
| 10   | set_sheet_of_light_param                  | 设置片光模型对应的参数                       | 68   |

## Chapter 6: 3D Tools(3D工具)

### 6.1 3D Object Model_3D 模型

| 序号 | 函数名                       | 函数说明及注释                          | 页码 |
| ---- | ---------------------------- | --------------------------------------- | ---- |
| 1    | affine_trans_object_model_3d | 应用校准变换到不一致的图像              | 73   |
| 2    | clear_all_object_model_3d    | 清除所有的片光模型，释放内存空间        | 73   |
| 3    | clear_object_model_3d        | 清除指定片光模型，释放内存空间          | 73   |
| 4    | copy_object_model_3d         | 创建一个基于3D测量的片光模型            | 73   |
| 5    | get_object_model_3d_params   | 提取一个3D对象模型的参数                | 73   |
| 6    | object_model_3d_to_xyz       | 把3D对象模型坐标变换到图像中            | 74   |
| 7    | prepare_object_model_3d      | 3D对象模型准备执行某一个操作            | 74   |
| 8    | project_object_model_3d      | 把一个3D对象模型的边沿投影到图像坐标中  | 74   |
| 9    | read_object_model_3d_dxf     | 读取一个3D对象模型，该文件格式为dxf格式 | 74   |
| 10   | write_object_model_3d        | 读取一个3D对象模型，该文件格式为dxf格式 | 74   |
| 11   | xyz_to_object_model_3d       | 把图像中对应的3D坐标转换到3D对象模型中  | 75   |

### 3D Segmentation_3D分割

| 序号 | 函数名                           | 函数说明及注释                   | 页码 |
| ---- | -------------------------------- | -------------------------------- | ---- |
| 1    | apply_sheet_of_light_calibration | 应用校准变换到不一致的图像       | 75   |
| 2    | segment_object_model_3d          | 清除所有的片光模型，释放内存空间 | 75   |

## Chapter 7: Calibration(校准)

### 7.1 Binocular 双目相机

| 序号 | 函数名                | 函数说明及注释       | 页码 |
| ---- | --------------------- | -------------------- | ---- |
| 1    | binocular_calibration | 测试双目相机系统参数 | 79   |

### 3D Segmentation_3D分割

| 序号 | 函数名              | 函数说明及注释                                         | 页码 |
| ---- | ------------------- | ------------------------------------------------------ | ---- |
| 1    | caltab_points       | 从标定板文件中读取标志的中心点                         | 79   |
| 2    | create_caltab       | 创建一个标定板描述文件和附加文件                       | 80   |
| 3    | disp_caltab         | 投射和视觉化图像中标定板的三维模型                     | 80   |
| 4    | find_caltab         | 在图像中根据标定板找出对应的区域                       | 80   |
| 5    | find_marks_and_pose | 从图像中提取二维校准标志和外部计算机参数来计算内部数值 | 80   |
| 6    | gen_caltab          | 创建一个标定板文件和相应的附文件                       | 81   |
| 7    | sim_caltab          | 根据标定板模拟一副图像                                 | 81   |

### 7.3 Camera Parameters 相机参数

| 序号 | 函数名             | 函数说明及注释                   | 页码 |
| ---- | ------------------ | -------------------------------- | ---- |
| 1    | cam_mat_to_cam_par | 从相机矩阵来获取的内部相机参数   | 81   |
| 2    | cam_par_to_cam_mat | 从相机内存参数来获取一个相机矩阵 | 81   |
| 3    | read_cam_par       | 从文本文件中读取内部相机参数     | 81   |
| 4    | write_cam_par      | 将内部相机参数写入文本文件中     | 82   |

### 7.4 Hand-Eye 手眼校正（机械手视觉校正）

| 序号 | 函数名               | 函数说明及注释   | 页码 |
| ---- | -------------------- | ---------------- | ---- |
| 1    | hand_eye_calibration | 执行一个手眼校准 | 82   |

### 7.5 Monocular 单目镜

| 序号 | 函数名             | 函数说明及注释                         | 页码 |
| :--- | ------------------ | -------------------------------------- | ---- |
| 1    | camera_calibration | 测顶同时发生的最小化程序的所有相机参数 | 82   |
| 2    | project_3d_point   | 将三维点投射到子像素图像坐标           | 83   |

### 7.6 Multi-View 多视角（校准或者矫正）

| 序号 | 函数名                          | 函数说明及注释                                       | 页码 |
| ---- | ------------------------------- | ---------------------------------------------------- | ---- |
| 1    | calibrate_cameras               | 矫正相机                                             | 83   |
| 2    | clear_all_calib_data            | 清除所有的矫正数据模型，释放内存空间                 | 83   |
| 3    | clear_all_camera_setup_models   | 清除所有的相机设备模式，释放内存空间                 | 84   |
| 4    | clear_calib_data                | 清除指定的矫正数据模型，释放内存空间                 | 84   |
| 5    | clear_camera_setup_model        | 清除指定的相机设备模式，释放内存空间                 | 84   |
| 6    | create_calib_data               | 创建一个矫正数据模型                                 | 84   |
| 7    | create_camera_setup_model       | 创建一个相机设备模式                                 | 84   |
| 8    | get_calib_data                  | 提取矫正数据模型参数                                 | 84   |
| 9    | get_calib_data_observ_points    | 提取标定板上圆点的中心坐标和各个校正目标物体的坐标系 | 84   |
| 10   | get_camera_setup_param          | 提取相机设备模式的参数                               | 85   |
| 11   | query_calib_data_observ_indices | 获取指定的（相机对应的被测）                         | 85   |
| 12   | read_calib_data                 | 读取矫正数据模型对应的文件                           | 85   |
| 13   | read_camera_setup_model         | 读取相机设备模式对应的文件                           | 85   |
| 14   | set_calib_data                  | 配置矫正数据模型                                     | 85   |
| 15   | set_calib_data_calib_object     | 指定矫正对象                                         | 86   |
| 16   | set_calib_data_cam_param        | 相机的类型，初始化相机内存参数                       | 86   |
| 17   | set_calib_data_observ_points    | 设置标定板上圆点的中心坐标和各个校正目标物体的坐标系 | 86   |
| 18   | set_camera_setup_cam_param      | 设置相机设备模式，默认类型，参数和相等坐标点         | 87   |
| 19   | set_cameras_setup_param         | 配置相机设备模式参数                                 | 87   |
| 20   | write_calib_data                | 保存矫正数据模型到一个文件中                         | 87   |
| 21   | write_camera_setup_model        | 保存相机设备模式参数到一个文件中                     | 87   |

### 7.7 Rectification 矫正

| 序号 | 函数名                                | 函数说明及注释                                 | 页码 |
| ---- | ------------------------------------- | ---------------------------------------------- | ---- |
| 1    | change_radial_distortion_cam_par      | 依照测定的径向畸变决定相机的新参数             | 87   |
| 2    | change_radial_distortion_contours_xld | 矫正轮廓的畸变                                 | 88   |
| 3    | change_radial_distortion_image        | 矫正图像的畸变                                 | 88   |
| 4    | change_radial_distortion_points       | 矫正像素坐标的畸变                             | 88   |
| 5    | contour_to_world_plane_xld            | 把xld轮廓转为大地坐标系统，z轴为0，即没有z轴   | 88   |
| 6    | gen_image_to_world_plane_map          | 生成一张投影图，在大地坐标系中描绘该图像的映射 | 88   |
| 7    | gen_radial_distortion_map             | 生成一张投影图，改变图像像素的径向畸变         | 89   |
| 8    | image_points_to_world_plane           | 在大地坐标系中变换图像像素点                   | 89   |
| 9    | image_to_world_plane                  | 矫正一副图像，把它转换为大地坐标               | 89   |

### 7.8 Self-Calibration 自动矫正

| 序号 | 函数名                             | 函数说明及注释                 | 页码 |
| ---- | ---------------------------------- | ------------------------------ | ---- |
| 1    | radial_distortion_self_calibration | 校准畸变                       | 89   |
| 2    | radiometric_self_calibration       | 矫正相机曝光                   | 90   |
| 3    | stationary_camera_self_calibration | 对已经固定的照相机执行自动矫正 | 90   |

## Chapter 8: Classification(分类)

### 8.1 Gaussian-Mixture-Models 高斯混合模型

| 序号 | 函数名                   | 函数说明及注释                                     | 页码 |
| ---- | ------------------------ | -------------------------------------------------- | ---- |
| 1    | add_sample_class_gmm     | 把一个模型范本添加到一个高斯混合模型的范本数据库上 | 95   |
| 2    | classify_class_gmm       | 通过一个高斯混合模型来计算一个特征向量的类         | 95   |
| 3    | clear_all_class_gmm      | 清除所有高斯混合模型                               | 95   |
| 4    | clear_class_gmm          | 清除一个高斯混合模型                               | 95   |
| 5    | clear_samples_class_gmm  | 清除一个高斯混合模型的范本数据库                   | 95   |
| 6    | create_class_gmm         | 创建一个高斯混合模型分类                           | 96   |
| 7    | evaluate_class_gmm       | 通过一个高斯混合模型评价一个特征向量               | 96   |
| 8    | get_params_class_gmm     | 提取一个高斯混合模型的参数                         | 96   |
| 9    | get_prep_info_class_gmm  | 提取一个高斯混合模型的预处理特征向量的信息内容     | 96   |
| 10   | get_sample_class_gmm     | 提取一个高斯混合模型的模型范本                     | 96   |
| 11   | get_sample_num_class_gmm | 提取一个高斯混合模型的样品模型的数量               | 97   |
| 12   | read_class_gmm           | 从一个文件中读取一个高斯混合模型                   | 97   |
| 13   | read_samples_class_gmm   | 从一个文件中读取一个高斯混合模型范本               | 97   |
| 14   | train_class_gmm          | 训练一个高斯混合模型                               | 97   |
| 15   | write_class_gmm          | 向一个文件中写入高斯混合模型                       | 97   |
| 16   | write_samples_class_gmm  | 向一个文件中写入高斯混合模型的范本数据             | 97   |

### 8.2 Hyperboxed 分类器

| 序号 | 函数名                   | 函数说明及注释                       | 页码 |
| ---- | ------------------------ | ------------------------------------ | ---- |
| 1    | clear_sampset            | 释放一个数据集                       | 98   |
| 2    | close_all_class_box      | 关闭所有分类器                       | 98   |
| 3    | close_class_box          | 关闭指定分类器                       | 98   |
| 4    | create_class_box         | 创建一个新的分类器                   | 98   |
| 5    | descript_class_box       | 分类器的描述                         | 98   |
| 6    | enquire_class_box        | 为一组属性分类                       | 98   |
| 7    | enquire_reject_class_box | 为一组带抑制类的属性分类             | 98   |
| 8    | get_class_box_param      | 获取分类器对应的参数信息             | 98   |
| 9    | learn_class_box          | 分类器范本                           | 99   |
| 10   | learn_sampset_box        | 用数据组指定分类器范本               | 99   |
| 11   | read_class_box           | 从一个文件中读取分类器               | 99   |
| 12   | read_sampset             | 从一个文件中读取一个分类器范本数据集 | 99   |
| 13   | set_class_box_param      | 为分类器设置系统参数                 | 99   |
| 14   | test_sampset_box         | 为一组数组分类                       | 99   |
| 15   | write_class_box          | 将分类器保存到文件中                 | 99   |

### 8.3 Look_Up Table 颜色查询表

| 序号 | 函数名               | 函数说明及注释                                    | 页码 |
| ---- | -------------------- | ------------------------------------------------- | ---- |
| 1    | clear_all_class_lut  | 清除所有的颜色查找表分类器                        | 100  |
| 2    | clear_class_lut      | 清除指定的颜色查找表分类器                        | 100  |
| 3    | create_class_lut_gmm | 产生一个基于高斯矩阵模型（gmm）的颜色查找表分类器 | 100  |
| 4    | create_class_lut_mlp | 产生一个基于多层感知器（mlp）的颜色查找表分类器   | 100  |
| 5    | create_class_lut_svn | 产生一个基于支持向量机（svm）的颜色查找表分类器   | 100  |

### 8.4 Neural-Nets 感知网络

| 序号 | 函数名                   | 函数说明及注释                               | 页码 |
| ---- | ------------------------ | -------------------------------------------- | ---- |
| 1    | add_sample_class_mlp     | 把一个范文添加到一个多层感知器的范本数据集中 | 101  |
| 2    | classify_class_mlp       | 通过一个多层感知器计算一个特征向量的类       | 101  |
| 3    | clear_all_class_mlp      | 清除所有多层感知器                           | 101  |
| 4    | clear_class_mlp          | 清除一个指定的多层感知器                     | 101  |
| 5    | clear_samples_class_mlp  | 清除一个多层感知器的范本数据                 | 101  |
| 6    | create_class_mlp         | 为样式分类创建一个多层感知器                 | 102  |
| 7    | evaluate_class_mlp       | 通过一个多层感知器计算一个特征向量的评估     | 102  |
| 8    | get_params_class_mlp     | 提取一个多层感知器的参数                     | 102  |
| 9    | get_prep_info_class_mlp  | 提取一个多层感知器的预处理特征向量的信息内容 | 102  |
| 10   | get_sample_class_mlp     | 提取一个多层感知器的范本                     | 102  |
| 11   | get_sample_num_class_mlp | 提取一个多层感知器的范本数量                 | 102  |
| 12   | read_class_mlp           | 从一个文件中读取一个多层感知器               | 102  |
| 13   | read_samples_class_mlp   | 从一个文件中读取一个多层感知器的范本数据     | 103  |
| 14   | train_class_mlp          | 训练多层感知器                               | 103  |
| 15   | write_class_mlp          | 向一个文件中写入一个多层感知器               | 103  |
| 16   | write_samples_classs_mlp | 向一个文件中写入一个多层感知器的范本数据     | 103  |

### 8.5 Support-Vector-Machines 矢量

| 序号 | 函数名                           | 函数说明及注释                                               | 页码 |
| ---- | -------------------------------- | ------------------------------------------------------------ | ---- |
| 1    | add_sample_class_svm             | 把一个范本添加到一个支持向量机的训练数据上                   | 104  |
| 2    | classify_class_svm               | 通过一个支持向量机为一个特征向量分类                         | 104  |
| 3    | clear_all_class_svm              | 清除所有支持向量机                                           | 104  |
| 4    | clear_class_svm                  | 清除一个支持向量机                                           | 104  |
| 5    | clear_samples_class_svm          | 清除一个支持向量机的范本数据                                 | 104  |
| 6    | create_class_svm                 | 为模式分类创建一个支持向量机                                 | 104  |
| 7    | get_params_class_svm             | 提取一个支持向量机的参数                                     | 105  |
| 8    | get_prep_info_class_svm          | 提取一个支持向量机的预处理特征向量的信息内容                 | 105  |
| 9    | get_sample_class_svm             | 提取一个支持向量机的范本                                     | 105  |
| 10   | get_sample_num_class_svm         | 提取一个支持向量机范本的数量                                 | 105  |
| 11   | get_support_vector_class_svm     | 提取一个支持向量机范本的索引                                 | 105  |
| 12   | get_support_vector_num_class_svm | 提取一个支持向量机中支持向量的数量                           | 105  |
| 13   | read_class_svm                   | 从一个文件中读取一个支持向量机                               | 106  |
| 14   | read_samples_class_svm           | 从一个文件中读取一个支持向量机的范本数据                     | 106  |
| 15   | reduce_class_svm                 | 根据一个简化的支持向量机来近似一个范本的支持向量机（为了更快分类） | 106  |
| 16   | train_class_svm                  | 训练一个支持向量机模型                                       | 106  |
| 17   | write_class_svm                  | 向一个文件中写入一个支持向量机                               | 106  |
| 18   | write_samples_class_svm          | 向一个文件中写入一个支持向量机的示范数据                     | 106  |

## Chapter 9: File(文件)

### 9.1 Images  图像

| 序号 | 函数名           | 函数说明及注释                   | 页码 |
| ---- | ---------------- | -------------------------------- | ---- |
| 1    | read_image       | 读取不同文件格式的图像           | 109  |
| 2    | read_sequence    | 读取图像                         | 109  |
| 3    | write_image      | 用图形格式写图像                 | 109  |
| 4    | list_image_files | 获取所有图像文件的目录           | 109  |
| 5    | parse_filename   | 获取图像的文件描述，后缀名及目录 | 109  |

### 9.2 Misc 混合体

| 序号 | 函数名          | 函数说明及注释                       | 页码 |
| ---- | --------------- | ------------------------------------ | ---- |
| 1    | delete_file     | 删除一个文件                         | 110  |
| 2    | file_exists     | 检查文件是否存在                     | 110  |
| 3    | list_files      | 列出目录中的所有文件                 | 111  |
| 4    | read_world_file | 从一个ARC/INFO世界文件中读取地理编码 | 111  |

### 9.3 Region 区域

| 序号 | 函数名       | 函数说明及注释             | 页码 |
| ---- | ------------ | -------------------------- | ---- |
| 1    | read_region  | 读取二值图像或者HALCON区域 | 111  |
| 2    | write_region | 在文件中写入区域           | 112  |

### 9.4 Text 文

| 序号 | 函数名          | 函数说明及注释               | 页码 |
| ---- | --------------- | ---------------------------- | ---- |
| 1    | close_all_files | 关闭所有打开的文件           | 112  |
| 2    | close_file      | 关闭一个文本文件             | 112  |
| 3    | fnew_line       | 创建一个换行符               | 112  |
| 4    | fread_char      | 从一个文本文件中读取一个字符 | 112  |
| 5    | fread_line      | 从一个文本文件中读取一行     | 113  |
| 6    | fread_string    | 从一个文本文件中读取字符串   | 113  |
| 7    | fwrite_string   | 向一个文本文件中写入值       | 113  |
| 8    | open_file       | 打开文本文件                 | 113  |

### 9.5 Tuple 数组

| 序号 | 函数名      | 函数说明及注释           | 页码 |
| ---- | ----------- | ------------------------ | ---- |
| 1    | read_tuple  | 从一个文件中读取一个数组 | 113  |
| 2    | write_tuple | 向一个文件中写入一个数组 | 114  |

### 9.6 XLD

| 序号 | 函数名                     | 函数说明及注释                                | 页码 |
| ---- | -------------------------- | --------------------------------------------- | ---- |
| 1    | read_contour_xld_arc_info  | 从用ARC/INFO生成格式表示的文件读取XLD轮廓     | 114  |
| 2    | read_contour_xld_dxf       | 从一个DXF文件汇总读取XLD轮廓。DXF:CAD绘图格式 | 114  |
| 3    | read_polygon_xld_arc_info  | 从用ARC/INFO生成格式表示的文件读取XLD多边形   | 114  |
| 4    | read_polygon_xld_dxf       | 从一个DXF文件中读取XLD多边形                  | 115  |
| 5    | write_contour_xld_arc_info | 向用ARC/INFO生成格式表示的文件写入XLD轮廓     | 115  |
| 6    | write_contour_xld_dxf      | 向一个DXF格式的文件中写入XLD轮廓              | 115  |
| 7    | write_polygon_xld_arc_info | 向用ARC/INFO生成格式表示的文件写入XLD多边形   | 115  |
| 8    | write_polygon_xld_dxf      | 向一个DXF格式的文件中写入XLD多边形            | 115  |

## Chapter 10: Filter(过滤)

### 10.1 Arithmetic 图像算数处理

| 序号 | 函数名         | 函数说明及注释               | 页码 |
| ---- | -------------- | ---------------------------- | ---- |
| 1    | abs_diff_image | 计算两个图像的绝对差别       | 119  |
| 2    | abs_image      | 计算一个图像的绝对值（模数） | 119  |
| 3    | add_image      | 使两个图像相加               | 120  |
| 4    | div_image      | 使两个图像相除               | 120  |
| 5    | invert_image   | 使一个图像反像               | 121  |
| 6    | max_image      | 按像素计算两个图像的最大值   | 121  |
| 7    | min_image      | 按像素计算两个图像的最小值   | 121  |
| 8    | mult_image     | 使两个图像相乘               | 122  |
| 9    | scale_image    | 为一个图像的灰度值分级       | 122  |
| 10   | sqrt_image     | 计算一个图像的平方根         | 123  |
| 11   | sub_image      | 使两个图像相减               | 123  |

### 10.2 Bit 图位像素处理

| 序号 | 函数名     | 函数说明及注释                   | 页码 |
| ---- | ---------- | -------------------------------- | ---- |
| 1    | bit_and    | 输入图像对应的所有像素的逐位与   | 124  |
| 2    | bit_lshift | 图像对应的所有像素的左移         | 124  |
| 3    | bit_mask   | 使用位掩码对每个像素的逻辑与     | 125  |
| 4    | bit_not    | 对像素的所有位进行求补           | 125  |
| 5    | bit_or     | 输入图像对应的所有像素的逐位或   | 125  |
| 6    | bit_rshift | 图像对应的所有像素的右移         | 126  |
| 7    | bit_slice  | 从像素中提取一位                 | 126  |
| 8    | bit_xor    | 输入图像对应的所有像素的逐位异或 | 127  |

### 10.3 Color图像颜色处理

| 序号 | 函数名                     | 函数说明及注释                                       | 页码 |
| ---- | -------------------------- | ---------------------------------------------------- | ---- |
| 1    | apply_color_trans_lut      | 申请使用颜色查找表（lut）                            | 127  |
| 2    | cfa_to_rgb                 | 把一个单通道颜色滤波阵列图像（带RGB成分）变成RGB图像 | 127  |
| 3    | clear_all_color_trans_luts | 清除所有的颜色查找表，释放内存空间                   | 127  |
| 4    | clear_color_trans_lut      | 清除颜色查找表，释放内存空间                         | 128  |
| 5    | create_color_trans_lut     | 创建一个颜色查询表，该表为RGB图像提供转换服务        | 128  |
| 6    | gen_principal_comp_trans   | 计算多通道图像的PCA（主要部分分析）的转换矩阵        | 128  |
| 7    | linear_trans_color         | 计算多通道图像的颜色值的一个仿射变换                 | 128  |
| 8    | principal_comp             | 计算多通道图像的PCA（主要部分分析）                  | 128  |
| 9    | rgb1_to_gray               | 把一个RGB图像转变成一个灰度图像                      | 128  |
| 10   | rgb3_to_gray               | 把一个RGB图像转变成一个灰度图像                      | 128  |
| 11   | trans_from_rgb             | 把一个图像从RGB颜色空间转变成任意颜色空间            | 129  |
| 12   | trans_to_rgb               | 把一个图像从任意颜色空间转变成RGB颜色空间            | 129  |

### 10.4 Edges 图像边沿处理

| 序号 | 函数名              | 函数说明及注释                                             | 页码 |
| ---- | ------------------- | ---------------------------------------------------------- | ---- |
| 1    | close_edges         | 使用边缘幅值图像清除边缘缺陷                               | 131  |
| 2    | close_edges_length  | 使用边缘幅值图像清除边缘缺陷                               | 131  |
| 3    | derivate_gauss      | 用高斯派生物对一个图像卷积                                 | 132  |
| 4    | diff_of_gauss       | 近似高斯的拉普拉斯算子                                     | 133  |
| 5    | edges_color         | 使用Canny、Deriche或者Shen滤波器提取颜色边缘               | 133  |
| 6    | edges_color_sub_pix | 使用Canny、Deriche或者Shen滤波器提取子像素精确颜色边缘     | 134  |
| 7    | edges_image         | 使用Deriche、Lanser、Shen或者Canny滤波器提取边缘           | 134  |
| 8    | edges_sub_pix       | 使用Deriche、Lanser、Shen或者Canny滤波器提取子像素精确边缘 | 135  |
| 9    | frei_amp            | 使用Frei-Chen算子检测边缘（幅值）                          | 136  |
| 10   | frei_dir            | 使用Frei-Chen算子检测边缘（幅值和相位）                    | 136  |
| 11   | highpass_image      | 从一个图像提取高频成分                                     | 137  |
| 12   | info_edges          | 在edges_image估计滤波器的宽度                              | 137  |
| 13   | kirsch_amp          | 使用Kirsch算子检测边缘（幅值）                             | 138  |
| 14   | kirsch_dir          | 使用Kirsch算子检测边缘（幅值和相位）                       | 138  |
| 15   | laplace             | 使用有限差计算拉普拉斯算子                                 | 139  |
| 16   | laplace_of_gauss    | 高斯的拉普拉斯算子                                         | 139  |
| 17   | prewitt_amp         | 使用Prewitt算子检测边缘（幅值）                            | 140  |
| 18   | prewitt_dir         | 使用Prewitt算子检测边缘（幅值和相位）                      | 140  |
| 19   | roberts             | 使用Roberts滤波器检测边缘                                  | 141  |
| 20   | robinson_amp        | 使用Robinson算子检测边缘（幅值）                           | 141  |
| 21   | robinson_dir        | 使用Robinson算子检测边缘（幅值和相位）                     | 142  |
| 22   | sobel_amp           | 使用Sobel算子检测边缘（幅值）                              | 142  |
| 23   | sobel_dir           | 使用Sobel算子检测边缘（幅值和相位）                        | 143  |

### 10.5 Enhancement 增强图形

| 序号 | 函数名                   | 函数说明及注释                         | 页码 |
| ---- | ------------------------ | -------------------------------------- | ---- |
| 1    | coherence_enhancing_diff | 执行图像的一致性增强扩散               | 143  |
| 2    | emphasize                | 增强图像对比度                         | 144  |
| 3    | equ_histo_image          | 图像的柱状线性比                       | 144  |
| 4    | illuminate               | 增强图像对比度                         | 145  |
| 5    | mean_curvature_flow      | 把平均曲率应用在一个图像中             | 145  |
| 6    | scale_image_max          | 增强图像反差，最大灰度值在0到255范围内 | 146  |
| 7    | shock_filter             | 把一个冲击滤波器应用到一个图像中       | 146  |

### 10.6 FFT快速博氏变换算法

| 序号 | 函数名                      | 函数说明及注释                            | 页码 |
| ---- | --------------------------- | ----------------------------------------- | ---- |
| 1    | convol_fft                  | 用在频域内的滤波器使一个图像卷积          | 148  |
| 2    | convol_gabor                | 用在频域内的一个Gabor滤波器使一个图像卷积 | 148  |
| 3    | correlation_ffg             | 计算在频域内的两个图像的相互关系          | 148  |
| 4    | energy_gabor                | 计算一个两通道图像的能量                  | 149  |
| 5    | fft_generic                 | 计算一个图像的快速傅里叶变换              | 149  |
| 6    | fft_image                   | 计算一个图像的快速傅里叶变换              | 149  |
| 7    | fft_image_inv               | 计算一个图像的快速傅里叶逆变换            | 150  |
| 8    | gen_bandfilter              | 生成一个理想带状滤波器                    | 150  |
| 9    | gen_bandpass                | 生成一个理想带通滤波器                    | 151  |
| 10   | gen_derivative_filter       | 在频域内生成一个派生滤波器                | 151  |
| 11   | gen_filter_mask             | 在空域内存储一个滤波器掩码作为实时图像    | 152  |
| 12   | gen_gabor                   | 生成一个Gabor滤波器                       | 153  |
| 13   | gen_gauss_filter            | 在频域内生成一个高斯滤波器                | 153  |
| 14   | gen_highpass                | 生成一个理想高通滤波器                    | 154  |
| 15   | gen_lowpass                 | 生成一个理想低通滤波器                    | 154  |
| 16   | gen_mean_filter             | 生成一个均值滤波器                        | 155  |
| 17   | gen_sin_bandpass            | 用正弦形状生成一个带通滤波器              | 155  |
| 18   | gen_std_bandpass            | 用高斯或者正弦形状生成一个带通滤波器      | 156  |
| 19   | optimize_fft_speed          | 使FFT的运行时间最优化                     | 156  |
| 20   | optimize_rft_speed          | 使实值的FFT的运行时间最优化               | 156  |
| 21   | phase_deg                   | 返回用角度表示一个复杂图像的相位          | 157  |
| 22   | phase_rad                   | 返回用弧度表示一个复杂图像的相位          | 157  |
| 23   | power_byte                  | 返回一个复杂图像的功率谱                  | 157  |
| 24   | power_ln                    | 返回一个复杂图像的功率谱                  | 158  |
| 25   | power_real                  | 返回一个复杂图像的功率谱                  | 158  |
| 26   | read_fft_optimization_data  | 从一个文件中下载FFT速度最优数据           | 158  |
| 27   | rft_generic                 | 计算一个图像的实值快速傅里叶变换          | 158  |
| 28   | write_fft_optimization_data | 把FFT速度最优数据存储在一个文件中         | 159  |

### 10.7 Geometric-Transformations 图像几何变换

| 序号 | 函数名                      | 函数说明及注释                                   | 页码 |
| ---- | --------------------------- | ------------------------------------------------ | ---- |
| 1    | affine_trans_image          | 把任意仿射2D变换应用在图像中                     | 159  |
| 2    | affine_trans_image_size     | 把任意仿射2D变换应用在图像中并且指定输出图像大小 | 160  |
| 3    | convert_map_type            | 将图像转换为其它类型                             | 161  |
| 4    | map_image                   | 把一个一般变换应用于一个图像中                   | 161  |
| 5    | mirror_image                | 镜像一个图像                                     | 162  |
| 6    | polar_trans_image           | 把一个图像转换成极坐标                           | 162  |
| 7    | polar_trans_image_ext       | 把一个图像中的环形弧转变成极坐标                 | 162  |
| 8    | polar_trans_image_inv       | 把极坐标中的图像转变成直角坐标                   | 163  |
| 9    | projective_trans_image      | 把投影变换应用于一个图像中                       | 164  |
| 10   | projective_trans_image_size | 把投影变换应用于一个图像中并且指定输出图像的大小 | 165  |
| 11   | rotate_image                | 以一个图像的中心为圆心旋转                       | 166  |
| 12   | zoom_image_factor           | 把一个图像缩放到指定比例大小                     | 166  |
| 13   | zoom_image_size             | 把一个图像缩放到指定大小                         | 166  |

### 10.8 Inpainting 图像修复

| 序号 | 函数名                 | 函数说明及注释                 | 页码 |
| ---- | ---------------------- | ------------------------------ | ---- |
| 1    | harmonic_interpolation | 对一个图像区域执行谐波插值     | 167  |
| 2    | inpainting_aniso       | 通过各向异性扩散执行图像修复   | 168  |
| 3    | inpainting_ced         | 通过一致性增强扩散执行图像修复 | 168  |
| 4    | inpainting_ct          | 通过连贯传送执行图像修复       | 169  |
| 5    | inpainting_mcf         | 通过水平线平滑执行图像修复     | 169  |
| 6    | inpainting_texture     | 通过结构传导执行图像修复       | 170  |

### 10.9 Lines 色线

| 序号 | 函数名         | 函数说明及注释         | 页码 |
| ---- | -------------- | ---------------------- | ---- |
| 1    | bandpass_image | 使用带通滤波器提取边缘 | 170  |
| 2    | lines_color    | 检测色线和它们的宽度   | 171  |
| 3    | lines_facet    | 使用面模型检测线       | 171  |
| 4    | lines_gauss    | 检测线和它们的宽度     | 172  |

### 10.10 Match 图像匹配

| 序号 | 函数名              | 函数说明及注释                       | 页码 |
| ---- | ------------------- | ------------------------------------ | ---- |
| 1    | exhaustive_match    | 模板和图像的匹配                     | 173  |
| 2    | exhaustive_match_mg | 在一个分辨率塔式结构中匹配模板和图像 | 173  |
| 3    | gen_gauss_pyramid   | 计算一个高斯金字塔                   | 174  |
| 4    | monotony            | 计算单调（无聊）操作                 | 174  |

### 10.11 Misc 混合

| 序号 | 函数名             | 函数说明及注释                                           | 页码 |
| ---- | ------------------ | -------------------------------------------------------- | ---- |
| 1    | convol_image       | 用一个任意滤波掩码对一个图像卷积                         | 175  |
| 2    | expand_domain_gray | 扩大图像区域并且在扩大的区域中设置灰度值                 | 175  |
| 3    | gray_inside        | 对图像中的每一点在图像边界的任意路径计算尽可能低的灰度值 | 176  |
| 4    | gray_skeleton      | 灰度值图像的细化                                         | 176  |
| 5    | lut_trans          | 使用灰度值查询表转换一个图像                             | 176  |
| 6    | symmetry           | 沿一行灰度值的对称性                                     | 177  |
| 7    | topographic_sketch | 计算一个图像的地理原始草图                               | 177  |

### 10.12 Noise 噪声

| 序号 | 函数名                  | 函数说明及注释         | 页码 |
| ---- | ----------------------- | ---------------------- | ---- |
| 1    | add_noise_distribution  | 向一个图像添加噪声     | 178  |
| 2    | add_noise_white         | 向一个图像添加噪声     | 178  |
| 3    | gauss_distribution      | 产生一个高斯噪声分布   | 178  |
| 4    | noise_distribution_mean | 测定一个图像的噪声分布 | 178  |
| 5    | sp_distribution         | 产生一个椒盐噪声分布   | 178  |

### 10.13 Optical-FLow 光流

| 序号 | 函数名                    | 函数说明及注释               | 页码 |
| ---- | ------------------------- | ---------------------------- | ---- |
| 1    | optical_flow_mg           | 计算两个图像之间的光流       | 178  |
| 2    | unwarp_image_vector_field | 使用一个矢量场来展开一个图像 | 179  |
| 3    | vector_field_length       | 计算一个矢量场的矢量长度     | 180  |

### 10.14 Points 角点

| 序号 | 函数名                 | 函数说明及注释            | 页码 |
| ---- | ---------------------- | ------------------------- | ---- |
| 1    | corner_response        | 在图像中寻找角点          | 180  |
| 2    | dots_image             | 在一个图像中增强圆形点    | 181  |
| 3    | points_foerstner       | 使用Foerstner算子检测角点 | 182  |
| 4    | points_harris          | 使用Harris算子检测角点    | 183  |
| 5    | points_harris_binomial | 使用Harris二项式找出角点  | 183  |
| 6    | points_lepetit         | 使用Lepetit算子找出角点   | 184  |
| 7    | points_sojka           | 使用Sojka算子找出角点     | 185  |

### 10.15 Smoothing  滤波处理

| 序号 | 函数名                | 函数说明及注释                     | 页码 |
| ---- | --------------------- | ---------------------------------- | ---- |
| 1    | anisotropic_diffusion | 对一个图像执行各向异性扩散         | 186  |
| 2    | binomial_filter       | 使用binomial滤波器平滑一个图像     | 186  |
| 3    | eliminate_min_max     | 在空域内平滑一个图像来抑制噪声     | 187  |
| 4    | eliminate_sp          | 用中值代替阀值外的值               | 187  |
| 5    | fill_interlace        | 插补两个对半视频图像               | 187  |
| 6    | gauss_image           | 使用离散高斯函数平滑图像           | 188  |
| 7    | info_smooth           | 平滑滤波器smooth_image的信息       | 188  |
| 8    | isotropic_diffusion   | 对一个图像执行各向同性扩散         | 188  |
| 9    | mean_image            | 通过均值平滑一个图像               | 189  |
| 10   | mean_n                | 几个通道的平均灰度值               | 189  |
| 11   | mean_sp               | 抑制椒盐噪声                       | 190  |
| 12   | median_image          | 使用不同级别掩码的中值滤波         | 190  |
| 13   | median_rect           | 使用中值平滑滤波图像（橡皮擦功能） | 191  |
| 14   | median_separate       | 使用矩形掩码的离散中值滤波         | 191  |
| 15   | median_weighted       | 使用不同级别掩码的加权中值滤波     | 192  |
| 16   | midrange_image        | 计算掩码内最大和最小值的平均       | 192  |
| 17   | rank_n                | 几个通道的平均灰度值               | 192  |
| 18   | rank_rect             | 通过一个矩形掩码平滑一个图像       | 193  |
| 19   | rank_image            | 通过一个任意等级掩码平滑一个图像   | 193  |
| 20   | sigma_image           | 使用sigma滤波器的非线性平滑        | 194  |
| 21   | smooth_image          | 使用递归滤波器平滑一个图像         | 194  |
| 22   | trimmed_mean          | 使用任意等级掩码平滑一个图像       | 195  |

### 10.16 Texture 图像质感

| 序号 | 函数名          | 函数说明及注释                                 | 页码 |
| ---- | --------------- | ---------------------------------------------- | ---- |
| 1    | deviation_image | 计算矩形窗口内的灰度值的标准偏差               | 195  |
| 2    | entropy_image   | 计算矩形窗口内的灰度值的平均信息量             | 196  |
| 3    | texture_laws    | 使用一个Laws文本滤波器（地质变形）过滤一个图像 | 196  |

### 10.17 Wiener-Filter 维纳滤波器

| 序号 | 函数名           | 函数说明及注释                     | 页码 |
| ---- | ---------------- | ---------------------------------- | ---- |
| 1    | gen_psf_defocus  | 产生一个均匀散焦模糊的脉冲相应     | 197  |
| 2    | gen_psf_motion   | 产生一个（线性）运动模糊的脉冲相应 | 197  |
| 3    | simulate_defocus | 对一个图像的均匀散焦模糊进行仿真   | 197  |
| 4    | simulate_motion  | （线性）运动模糊的仿真             | 198  |
| 5    | wiener_filter    | 通过Wiener滤波进行图像恢复         | 198  |
| 6    | wiener_filter_ni | 通过Wiener滤波进行图像恢复         | 198  |

## Chapter 11: Graphics(绘图)

### 11.1 Drawing  绘图

| 序号 | 函数名                | 函数说明及注释                    | 页码 |
| ---- | --------------------- | --------------------------------- | ---- |
| 1    | drag_region1          | 一个区域的交互运动                | 204  |
| 2    | drag_region2          | 一个带有定点规格区域的交互运动    | 204  |
| 3    | drag_region3          | 一个带有限制位置区域的交互运动    | 204  |
| 4    | draw_circle           | 一个圆的交互绘图                  | 204  |
| 5    | draw_circle_mod       | 一个圆的交互绘图                  | 205  |
| 6    | draw_ellipse          | 一个椭圆的交互绘图                | 205  |
| 7    | draw_ellipse_mod      | 一个椭圆的交互绘图                | 205  |
| 8    | draw_line             | 一根线的交互绘图                  | 205  |
| 9    | draw_line_mod         | 一根线的交互绘图                  | 206  |
| 10   | draw_nurbs            | 一个NURBS曲线的交互绘图           | 206  |
| 11   | draw_nurbs_interp     | 使用插值的一个NURBS曲线的交互绘图 | 206  |
| 12   | draw_nurbs_interp_mod | 使用插值的一个NURBS曲线的交互修正 | 206  |
| 13   | draw_nurbs_mod        | 一个NURBS曲线的交互修正           | 207  |
| 14   | draw_point            | 一个点的交互绘图                  | 207  |
| 15   | draw_point_mod        | 一个点的交互绘图                  | 208  |
| 16   | draw_polygon          | 一个多边形的交互绘图              | 208  |
| 17   | draw_rectangle1       | 画一个与坐标轴平行的矩形          | 208  |
| 18   | draw_rectangle1_mod   | 画一个与坐标轴平行的矩形          | 208  |
| 19   | draw_rectangle2       | 任意定向矩形的交互绘图            | 209  |
| 20   | draw_rectangle2_mod   | 任意定向矩形的交互绘图            | 209  |
| 21   | draw_region           | 一个闭合区域的交互绘图            | 209  |
| 22   | draw_xld              | 一个轮廓的交互绘图                | 209  |
| 23   | draw_xld_mod          | 一个轮廓的交互修正                | 209  |
| 24   | disp_3d_coord_system  | 显示3D坐标轴系统                  | 210  |

### 11.2 Gnuplot 区域（小块地皮）

| 序号 | 函数名                | 函数说明及注释                                           | 页码 |
| ---- | --------------------- | -------------------------------------------------------- | ---- |
| 1    | gnuplot_close         | 关闭所有打开的gunplot文件或者终止一个活动的gnuplot子流程 | 210  |
| 2    | gnuplot_open_file     | 为图像和控制量的可视化打开一个gnuplot文件                | 210  |
| 3    | gnuplot_open_pipe     | 为图像和控制量的可视化打开一个通道的gnuplot流程          | 210  |
| 4    | gnuplot_plot_ctrl     | 使用gnuplot显示控制量                                    | 210  |
| 5    | gnuplot_plot_funct_1d | 使用gnuplot显示控制量的功能                              | 210  |
| 6    | gunplot_plot_image    | 使用gnuplot使一个图像可视化                              | 210  |

### 11.3  LUT（颜色查找表）也就是调色板

| 序号 | 函数名        | 函数说明及注释               | 页码 |
| ---- | ------------- | ---------------------------- | ---- |
| 1    | disp_lut      | 调色板的图解                 | 211  |
| 2    | draw_lut      | 交互利用调色板               | 211  |
| 3    | get_fixed_lut | 为实际彩色图像获取固定调色板 | 211  |
| 4    | get_lut       | 获取现在的调色板             | 211  |
| 5    | get_lut_style | 获取调色板的修正参数         | 211  |
| 6    | query_lut     | 查询所有可得到的调色板       | 212  |
| 7    | set_fixed_lut | 为实际彩色图像固定调色板     | 212  |
| 8    | set_lut       | 设置调色板                   | 212  |
| 9    | set_lut_style | 改变调色板                   | 213  |
| 10   | write_lut     | 把调色板作为文件写入         | 213  |

### 11.4  Mouse 鼠标事件

| 序号 | 函数名                | 函数说明及注释                   | 页码 |
| ---- | --------------------- | -------------------------------- | ---- |
| 1    | get_mbutton           | 等待鼠标按下并返回鼠标按下的位置 | 213  |
| 2    | get_mbutton_sub_pix   | 等待鼠标按下并返回鼠标按下的位置 | 213  |
| 3    | get_mposition         | 查询鼠标位置                     | 213  |
| 4    | get_mposition_sub_pix | 查询鼠标位置                     | 213  |
| 5    | get_mshape            | 查询现有鼠标指针形状             | 214  |
| 6    | query_mshape          | 查询所有可得到的鼠标指针形状     | 214  |
| 7    | set_mshape            | 设置现在鼠标指针形状             | 214  |

### 11.5  Output 输出图案

| 序号 | 函数名            | 函数说明及注释                  | 页码 |
| ---- | ----------------- | ------------------------------- | ---- |
| 1    | disp_arc          | 在一个窗口中显示圆形弧          | 215  |
| 2    | disp_arrow        | 在一个窗口中显示箭头            | 215  |
| 3    | disp_channel      | 用指定通道显示图像              | 215  |
| 4    | disp_circle       | 在一个窗口中显示圆              | 215  |
| 5    | disp_color        | 显示一个彩色（RGB）图像         | 216  |
| 6    | disp_cross        | 在一个窗口中显示交叉            | 216  |
| 7    | disp_distribution | 显示一个噪声分布                | 216  |
| 8    | disp_ellipse      | 显示椭圆                        | 216  |
| 9    | disp_image        | 显示灰度值图像                  | 216  |
| 10   | disp_line         | 在窗口中画一条线                | 217  |
| 11   | disp_obj          | 显示图像目标（图像，区域，XLD） | 217  |
| 12   | disp_polygon      | 显示一个多边型                  | 217  |
| 13   | disp_rectangle1   | 显示水平矩形                    | 217  |
| 14   | disp_rectangle2   | 显示任意方向的矩形              | 217  |
| 15   | disp_region       | 在一个窗口中显示区域            | 218  |
| 16   | disp_xld          | 显示一个XLD物体                 | 218  |

### 11.6  Parameters 参数

| 序号 | 函数名           | 函数说明及注释                 | 页码 |
| ---- | ---------------- | ------------------------------ | ---- |
| 1    | get_comprise     | 获取一个图像矩阵的输出处理     | 219  |
| 2    | get_draw         | 获取区域填充模式               | 219  |
| 3    | get_fix          | 获取查询表的固定模式           | 219  |
| 4    | get_hsi          | 获取颜色的HSI编码              | 220  |
| 5    | get_icon         | 查询区域输出的图标             | 220  |
| 6    | get_insert       | 获取显示模式                   | 220  |
| 7    | get_line_approx  | 获取轮廓显示的近似误差         | 220  |
| 8    | get_line_style   | 获取轮廓边线的显示模型（线性） | 220  |
| 9    | get_line_width   | 获取轮廓显示的线宽             | 220  |
| 10   | get_line_paint   | 获取灰度值的显示模式           | 220  |
| 11   | get_part         | 获取图像部分                   | 220  |
| 12   | get_part_style   | 获取灰度值显示的插值模式       | 221  |
| 13   | get_pixel        | 获取查询表索引的颜色           | 221  |
| 14   | get_rgb          | 获取RGB编码中的颜色            | 221  |
| 15   | get_shape        | 获取区域输出形状               | 221  |
| 16   | get_window_param | 获取窗口设置参数的值           | 221  |
| 17   | query_all_colors | 查询所有颜色名称               | 221  |
| 18   | query_color      | 查询窗口中显示的所有颜色名称   | 221  |
| 19   | query_colored    | 查询颜色输出的颜色数目         | 221  |
| 20   | query_gray       | 查询显示的灰度值               | 222  |
| 21   | query_insert     | 查询可能的图解模式             | 222  |
| 22   | quert_line_width | 查询可能的线宽                 | 222  |
| 23   | query_paint      | 查询灰度值显示模式             | 222  |
| 24   | query_shape      | 查询区域显示模式               | 222  |
| 25   | set_color        | 设置输出颜色                   | 222  |
| 26   | set_colored      | 设置多输出颜色                 | 222  |
| 27   | set_comprise     | 定义图像矩阵输出剪辑           | 222  |
| 28   | set_draw         | 定义区域填充模式               | 223  |
| 29   | set_fix          | 设置固定的查询表               | 223  |
| 30   | set_gray         | 定义区域输出的灰度值           | 223  |
| 31   | set_hsi          | 定义输出颜色（HSI编码）        | 223  |
| 32   | set_icon         | 区域输出的图标定义             | 223  |
| 33   | set_insert       | 定义图像输出功能               | 223  |
| 34   | set_line_approx  | 定义输出新暗示的近似误差       | 223  |
| 35   | set_line_style   | 定义一个轮廓输出模式           | 223  |
| 36   | set_line_width   | 定义区域轮廓输出的线宽         | 224  |
| 37   | set_paint        | 定义灰度值输出模式             | 224  |
| 38   | set_part         | 修正显示图像部分               | 224  |
| 39   | set_part_style   | 为灰度值输出定义一个插值方法   | 224  |
| 40   | set_pixel        | 定义一个颜色查询表索引         | 224  |
| 41   | set_rgb          | 通过RGB值设置颜色定义          | 224  |
| 42   | set_shape        | 定义区域输出轮廓               | 224  |
| 43   | set_window_param | 设置窗口参数                   | 225  |

### 11.7 Text 文本

| 序号 | 函数名                | 函数说明及注释                     | 页码 |
| ---- | --------------------- | ---------------------------------- | ---- |
| 1    | get_font              | 获取现有字体                       | 226  |
| 2    | get_font_extents      | 获取所有字体的特征（最大值）       | 226  |
| 3    | get_string_extents    | 获取一个字符串的空间大小           | 226  |
| 4    | get_tposition         | 获取光标位置                       | 226  |
| 5    | get_tshape            | 获取文本光标的形状                 | 226  |
| 6    | new_line              | 设置下一行的开始文本光标的位置     | 227  |
| 7    | query_font            | 查询可得到的字体                   | 227  |
| 8    | query_tshape          | 查询文本光标的所有可得到的形状     | 227  |
| 9    | read_char             | 从一个文本窗口读取一个字符         | 227  |
| 10   | read_string           | 从一个文本窗口读取一个字符串       | 227  |
| 11   | set_font              | 设置文本输出的字体                 | 227  |
| 12   | set_tposition         | 设置文本光标的位置                 | 227  |
| 13   | set_tshape            | 设置文本光标的形状                 | 227  |
| 14   | write_string          | 在一个窗口中打印文本               | 227  |
| 15   | disp_continue_message | 在荧幕上显示暂停程序继续操作的信息 | 228  |
| 16   | disp_message          | 在指定位置显示字符信息             | 228  |
| 17   | set_diaplay_font      | 设置显示的字体                     | 228  |

### 11.8 Window 窗口

| 序号 | 函数名                | 函数说明及注释                               | 页码 |
| ---- | --------------------- | -------------------------------------------- | ---- |
| 1    | clear_rectangle       | 在输出窗口中删除一个矩形                     | 229  |
| 2    | clear_window          | 清除一个输出窗口                             | 229  |
| 3    | close_window          | 关闭一个输出窗口                             | 229  |
| 4    | copy_rectangle        | 在输出窗口间复制矩形内所有像素               | 229  |
| 5    | dump_window           | 把窗口内容写入一个文件                       | 229  |
| 6    | dump_window_image     | 在一个图像目标中写窗口内容                   | 230  |
| 7    | get_os_window_handle  | 获取操作系统图像处理                         | 230  |
| 8    | get_window_attr       | 获取窗口特征                                 | 230  |
| 9    | get_window_extents    | 一个窗口大小和位置的信息                     | 230  |
| 10   | get_window_pointer3   | 一个窗口像素数据的通道                       | 230  |
| 11   | get_window_type       | 获取窗口类型                                 | 231  |
| 12   | move_rectangle        | 在一个输出窗口内部复制                       | 231  |
| 13   | new_extern_window     | 在Windows_NT 下创建一个虚拟图形窗口          | 231  |
| 14   | open_textwindow       | 打开一个文本窗口                             | 231  |
| 15   | open_window           | 打开一个图形窗口                             | 231  |
| 16   | query_window_type     | 查询所有可得到的窗口类型                     | 232  |
| 17   | set_window_attr       | 设置窗口特征                                 | 232  |
| 18   | set_window_dc         | 设置一个虚拟图形窗口（WIndows_NT）的设计背景 | 232  |
| 19   | set_window_extents    | 修正一个窗口的位置和大小                     | 232  |
| 20   | set_window_type       | 指定一个窗口类型                             | 232  |
| 21   | slide_image           | 两个窗口缓冲区的交互输出                     | 232  |
| 22   | unproject_coordinates | 在3D窗口中计算图像坐标的点                   | 233  |
| 23   | update_window_pose    | 修正3D姿势                                   | 233  |

## Chapter 12 : Identification(鉴定)

### 12.1 Bar Code 条形码

| 序号 | 函数名                      | 函数说明及注释                                 | 页码 |
| ---- | --------------------------- | ---------------------------------------------- | ---- |
| 1    | clear_all_bar_code_models   | 清除所有条形码模型，释放其分配的存储空间       | 237  |
| 2    | clear_bar_code_model        | 清除一个条形码模型，释放相应的存储空间         | 237  |
| 3    | create_bar_code_model       | 创建一个条形码阅读器模型                       | 237  |
| 4    | decode_bar_code_rectangle2  | 检测和读取在一个矩形框内的一副图像条形码符号   | 238  |
| 5    | find_bar_code               | 检测和读取一副图像中条形码符号                 | 238  |
| 6    | get_bar_code_object         | 访问创建在搜寻或条形码符号解码过程中的对象图标 | 239  |
| 7    | get_bar_code_param          | 获取一个或多个描述条形码模式的参数             | 240  |
| 8    | get_bar_code_param_specific | 获取一个或多个描述条形码模式的特定参数         | 240  |
| 9    | get_bar_code_result         | 获取字母数字混合编码的结果                     | 240  |
| 10   | query_bar_code_params       | 获取对应的条形码有哪些特定的参数               | 240  |
| 11   | set_bar_code_param          | 设置条形码模型的选定参数                       | 240  |
| 12   | set_bar_code_param_specific | 设置条形码模型的特定参数                       | 241  |

### 12.2 Data Code 二维条形码

| 序号 | 函数名                        | 函数说明及注释                                             | 页码 |
| ---- | ----------------------------- | ---------------------------------------------------------- | ---- |
| 1    | clear_all_data_code_2d_models | 清除所有的二维条码模型并释放它们分配的存储空间             | 242  |
| 2    | clear_data_code_2d_model      | 清除一个二维条码模型并释放它分配的存储空间                 | 242  |
| 3    | create_data_code_2d_model     | 创建一个二维条形码阅读器模型                               | 242  |
| 4    | find_data_code_2d             | 检测和读取一副图像或测试的二维条码编码模式中的二维条码符号 | 242  |
| 5    | get_data_code_2d_objects      | 查询搜索二维条码符号过程中创建对象的图标                   | 243  |
| 6    | get_data_code_2d_param        | 获取一个或多个描述二维条码模型的参数                       | 243  |
| 7    | get_data_code_2d_results      | 搜索二维条码符号过程中累计的字母数字混合编码的结果         | 244  |
| 8    | query_data_code_2d_params     | 为一个二维数据模型获取通用参数或对象的名字                 | 244  |
| 9    | read_data_code_2d_model       | 从一个文件中读取一个二维条码模型并新建一个模型             | 244  |
| 10   | set_data_code_2d_param        | 设置二维条码模型的选定参数                                 | 244  |
| 11   | write_data_code_2d_model      | 讲一个二维条码模型写入一个文件                             | 246  |

## Chapter 13 : Image（图像）

### 13.1 Access 数据

| 序号 | 函数名                   | 函数说明及注释                                         | 页码 |
| ---- | ------------------------ | ------------------------------------------------------ | ---- |
| 1    | get_grayval              | 获取一个图像目标（坐标）的灰度值                       | 251  |
| 2    | get_grayval_contour_xld  | 获取一个图像中XLD轮廓区域内的灰度值                    | 251  |
| 3    | get_grayval_interpolated | 获取一个图像指定位置的灰度值                           | 251  |
| 4    | get_image_pointer1       | 获取一个通道的指针                                     | 251  |
| 5    | get_image_pointer1_rect  | 获取图像数据指针和输入图像区域内最小矩形内部的图像数据 | 251  |
| 6    | get_image_pointer3       | 获取一个彩色图像的指针                                 | 252  |
| 7    | get_image_size           | 获取图像的大小                                         | 252  |
| 8    | get_image_time           | 获取图像创建的时间                                     | 252  |
| 9    | get_image_type           | 获取图像的类型                                         | 253  |

### 13.2 Acquisition 获取

| 序号 | 函数名                    | 函数说明及注释                                             | 页码 |
| ---- | ------------------------- | ---------------------------------------------------------- | ---- |
| 1    | close_all_framegrabbers   | 关闭所有图像获取设备                                       | 253  |
| 2    | close_framegrabber        | 关闭指定的图像获取设备                                     | 253  |
| 3    | get_framwgrabber_callback | 查找图像设备的回叫信号功能                                 | 253  |
| 4    | get_framegrabber_lut      | 查找图像获取设备的查询表                                   | 254  |
| 5    | get_framegrabber_param    | 查找一个图像获取设备的指定参数                             | 254  |
| 6    | grab_data                 | 从指定图像获取设备获取图像并且预处理该图像数据             | 254  |
| 7    | grab_data_async           | 从指定图像获取设备获取图像和图像数据并且开始下一个异步获取 | 255  |
| 8    | grab_image                | 从指定图像获取设备获取一个图像                             | 255  |
| 9    | grab_image_async          | 从指定图像获取设备获取一个图像并且开始下一步异步获取       | 255  |
| 10   | grab_image_start          | 从指定图像获取设备获取开始下一步异步获取                   | 255  |
| 11   | info_framegrabber         | 从指定图像获取设备查找信息                                 | 255  |
| 12   | open_framegrabber         | 打开并配置一个图像获取设备                                 | 256  |
| 13   | set_framegrabber_callback | 设置图像设备的回叫功能                                     | 257  |
| 14   | set_framegrabber_lut      | 设置图像获取设备查询表                                     | 257  |
| 15   | set_framegrabber_param    | 设置一个图像火土设备的指定参数                             | 257  |

### 13.3 Channel 设备途径

| 序号 | 函数名            | 函数说明及注释                     | 页码 |
| ---- | ----------------- | ---------------------------------- | ---- |
| 1    | access_channel    | 获取一个多通道图像的一个通道       | 258  |
| 2    | append_channel    | 把附加模型（通道）添加到图像上     | 258  |
| 3    | channels_to_image | 把单通道图像转变为一个多通道图像   | 258  |
| 4    | compose2          | 把两个图像转变为一个两通道图像     | 258  |
| 5    | compose3          | 把三个图像转变为一个三通道图像     | 258  |
| 6    | compose4          | 把四个图像转变为一个四通道图像     | 258  |
| 7    | compose5          | 把五个图像转变为一个五通道图像     | 258  |
| 8    | compose6          | 把六个图像转变为一个六通道图像     | 259  |
| 9    | compose7          | 把七个图像转变为一个七通道图像     | 259  |
| 10   | count_channels    | 计算图像的通道                     | 259  |
| 11   | decompose2        | 把一个两通道图像转变为两个图像     | 259  |
| 12   | decompose3        | 把一个三通道图像转变为三个图像     | 259  |
| 13   | decompose4        | 把一个四通道图像转变为四个图像     | 259  |
| 14   | decompose5        | 把一个五通道图像转变为五个图像     | 259  |
| 15   | decompose6        | 把一个六通道图像转变为六个图像     | 259  |
| 16   | decompose7        | 把一个七通道图像转变为七个图像     | 259  |
| 17   | image_to_channels | 把一个多通道图像转变为一个通道图像 | 259  |

### 13.4 Creation 创建

| 序号 | 函数名                         | 函数说明及注释                                   | 页码 |
| ---- | ------------------------------ | ------------------------------------------------ | ---- |
| 1    | copy_image                     | 复制一个图像并为它分配新内存                     | 260  |
| 2    | gen_image1                     | 从像素的一个指针创建一个图像                     | 260  |
| 3    | gen_image1_extern              | 从带存储管理的像素的一个指针创建一个图像         | 260  |
| 4    | gen_image1_rect                | 从像素（带存储管理）的指针创建一个矩形区域的图像 | 260  |
| 5    | gen_image3                     | 从像素（红、绿、蓝）的三个指针创建一个图像       | 260  |
| 6    | gen_image3_extern              | 从带存储管理的像素的一个指针创建一个图像         | 261  |
| 7    | gen_image_const                | 创建一个指定类型的（固定灰度值为0）图像          | 261  |
| 8    | gen_image_gray_ramp            | 创建一个灰度值阶梯                               | 261  |
| 9    | gen_image_interleaved          | 从交叉像素的一个指针创建一个三通道图像           | 262  |
| 10   | gen_image_proto                | 创建一个指定的固定灰度值的图像                   | 262  |
| 11   | gen_image_surface_first_order  | 创建一阶多项式的一个弯曲灰度表面                 | 263  |
| 12   | gen_image_surface_second_order | 创建二阶多项式的一个弯曲灰度表面                 | 263  |
| 13   | region_to_bin                  | 把一个区域转变为一个二进制字节图像               | 264  |
| 14   | region_to_label                | 把区域转变为一个标签图像                         | 265  |
| 15   | region_to_mean                 | 通过区域平均灰度值产生一个新图像                 | 265  |

### 13.5  Domain 区域

| 序号 | 函数名            | 函数说明及注释                   | 页码 |
| ---- | ----------------- | -------------------------------- | ---- |
| 1    | add_channels      | 在图形的指定区域中添加一个灰度值 | 265  |
| 2    | change_domain     | 改变一个图像的定义区间           | 266  |
| 3    | full_domain       | 把一个图像的区域扩大到最大值     | 266  |
| 4    | get_domain        | 获取一个图像的区域               | 266  |
| 5    | rectangle1_domain | 把一个图像的区域缩小到一个矩形   | 267  |
| 6    | reduce_domain     | 缩小一个图像的区域               | 267  |

### 13.6 Features 特征

| 序号 | 函数名                   | 函数说明及注释                                 | 页码 |
| ---- | ------------------------ | ---------------------------------------------- | ---- |
| 1    | area_center_gray         | 计算一个灰度值图像的区域面积和重心             | 268  |
| 2    | cooc_feature_image       | 计算一个同时出现的矩阵并得出相关灰度值特征     | 269  |
| 3    | cooc_feature_matrix      | 从一个同时出现的矩阵计算灰度值特征             | 269  |
| 4    | elliptic_axis_gray       | 在一个灰度值图像中计算一个区域的方位和主轴     | 269  |
| 5    | entropy_gray             | 确定一个图像的熵和各向异性                     | 270  |
| 6    | estimate_noise           | 从一个单一图像估计图像噪声                     | 270  |
| 7    | fit_surface_first_order  | 通过一个一阶表面（平面）计算灰度值力矩和近似值 | 270  |
| 8    | fit_surface_second_order | 通过一个二阶表面（平面）计算灰度值力矩和近似值 | 270  |
| 9    | fuzzy_entropy            | 确定区域的模糊熵（平均分布值）                 | 271  |
| 10   | fuzzy_perimeter          | 计算一个区域的模糊边缘周长                     | 271  |
| 11   | gen_cooc_matrix          | 在一个图像中计算一个区域中同时出现的矩阵       | 272  |
| 12   | gray_histo               | 计算灰度值分布                                 | 272  |
| 13   | gray_histo_abs           | 计算灰度值分布                                 | 273  |
| 14   | gray_histo_range         | 在指定范围内计算灰度值分布                     | 273  |
| 15   | gray_projections         | 计算水平和垂直灰度值预测                       | 273  |
| 16   | histo_2dim               | 计算两通道灰度值图像的直方图                   | 273  |
| 17   | intensity                | 计算灰度值的平均值和偏差                       | 273  |
| 18   | min_max_gray             | 计算区域内的最大和最小灰度值                   | 274  |
| 19   | moments_gray_plane       | 通过一个平面计算灰度值力矩和近似值             | 274  |
| 20   | plane_deviation          | 从近似像平面计算灰度值的偏差                   | 274  |
| 21   | select_gray              | 选择基于灰度值特征的区域                       | 274  |
| 22   | shape_histo_all          | 用极限值确定特征的一个直方图                   | 275  |
| 23   | shape_histo_point        | 用极限值确定特征的一个直方图                   | 275  |

### 13.7 Format 格式

| 序号 | 函数名             | 函数说明及注释                                 | 页码 |
| ---- | ------------------ | ---------------------------------------------- | ---- |
| 1    | change_format      | 改变图像大小                                   | 275  |
| 2    | crop_domain        | 修剪图像，对图像实际大小进行修剪               | 276  |
| 3    | crop_domain_rel    | 去掉和定义域有关的图像区域                     | 276  |
| 4    | crop_part          | 剪下一个矩形图像区域                           | 277  |
| 5    | crop_rectangle1    | 剪下一个矩形图像区域                           | 277  |
| 6    | tile_channels      | 把多重图像拼成一个大图像                       | 278  |
| 7    | tile_images        | 把多重图像目标拼成一个大图像                   | 278  |
| 8    | tile_images_offset | 把多重图像目标拼成一个有确定的位置信息的大图像 | 279  |

### 13.8 Manipulation （伪造，篡改图像）

| 序号 | 函数名           | 函数说明及注释                                         | 页码 |
| ---- | ---------------- | ------------------------------------------------------ | ---- |
| 1    | overpaint_gray   | 将源图像粘贴到目标图像里头去，重新绘制一个图像的灰度值 | 279  |
| 2    | overpaint_region | 重新绘制一个图像的区域，将区域采用指定灰度填充         | 280  |
| 3    | paint_gray       | 把一个图像的灰度值画在另一个图像上                     | 280  |
| 4    | paint_region     | 把区域画在一个图像中                                   | 281  |
| 5    | paint_xld        | 把XLD目标画在一个图像中                                | 281  |
| 6    | set_grayval      | 在一个图像中设置单灰度值                               | 282  |

### 13.9 Type-Conversion 类型变换

| 序号 | 函数名               | 函数说明及注释                     | 页码 |
| ---- | -------------------- | ---------------------------------- | ---- |
| 1    | complex_to_real      | 把一个复杂图像转变为两个实际图像   | 282  |
| 2    | convert_image_type   | 转变一个图像的类型                 | 283  |
| 3    | real_to_complex      | 把两个实际图像转变为一个复杂图像   | 283  |
| 4    | real_to_vector_field | 把两个实值图像转变为一个矢量域图像 | 283  |
| 5    | vector_field_to_real | 把一个矢量域图像转变为两个实值图像 | 284  |

## Chapter 14 : Inspection (检查)

### 14.1 OCV 字符识别检测

| 序号 | 函数名           | 函数说明及注释                    | 页码 |
| ---- | ---------------- | --------------------------------- | ---- |
| 1    | close_all_ocvs   | 关闭所有OCV工具，释放内存空间     | 288  |
| 2    | close_ocv        | 关闭一个OCV工具，释放内存空间     | 288  |
| 3    | create_ocv_proj  | 创建一个基于灰度值突出新的OCV工具 | 288  |
| 4    | do_ocv_simple    | 利用一个OCV工具查证一个模式       | 288  |
| 5    | read_ocv         | 从文件中读取一个OCV工具           | 288  |
| 6    | trained_ocv_proj | 测试一个OCV工具                   | 288  |
| 7    | write_ocv        | 将一个OCV工具保存到文件           | 288  |

### 14.2 Variation Model 变化模型

| 序号 | 函数名                            | 函数说明及注释                   | 页码 |
| ---- | --------------------------------- | -------------------------------- | ---- |
| 1    | clear_all_variation_models        | 释放所有变化模型的存储空间       | 289  |
| 2    | clear_train_data_variation_model  | 释放变化模型的测试数据的存储空间 | 289  |
| 3    | clear_variation_model             | 释放一个变化模型的存储空间       | 289  |
| 4    | compare_ext_variation_model       | 将一个图像与一个变化模型相比较   | 289  |
| 5    | compare_variation_model           | 将一个图像与一个变化模型相比较   | 289  |
| 6    | create_variation_model            | 创建一个用于图像对比的变化模型   | 289  |
| 7    | get_thresh_images_variation_model | 提取用于图像对比的阀值图像       | 290  |
| 8    | get_variation_model               | 返回图像用于图像对比             | 290  |
| 9    | prepare_direct_variation_model    | 为图像对比准备一个变化模型       | 290  |
| 10   | prepare_variation_model           | 为图像对比准备一个变化模型       | 290  |
| 11   | read_variation_model              | 从一个文件中读取一个变化模型     | 290  |
| 12   | train_variation_model             | 测试一个变化模型                 | 290  |
| 13   | write_variation_model             | 将一个变化模型写入文件           | 290  |

## Chapter 15 : Matching(匹配)

### 15.1 Component_Based 模件匹配

| 序号 | 函数名                         | 函数说明及注释                                         | 页码 |
| ---- | ------------------------------ | ------------------------------------------------------ | ---- |
| 1    | clear_all_component_models     | 释放所有组件匹配模型                                   | 293  |
| 2    | clear_all_training_components  | 释放所有组件模型                                       | 293  |
| 3    | clear_component_model          | 释放一个组件匹配模型                                   | 293  |
| 4    | clear_training_components      | 释放一个组件模型                                       | 293  |
| 5    | cluster_model_components       | 用于创建模型组件范本结果的新参数                       | 293  |
| 6    | create_component_model         | 创建一个组件匹配模型                                   | 294  |
| 7    | create_trained_component_model | 基于组件模型来创建一个组件匹配模型                     | 294  |
| 8    | find_component_model           | 在一个图像中搜索最佳组件匹配模型                       | 295  |
| 9    | gen_initial_components         | 提取一个组件模型的最初组件                             | 296  |
| 10   | get_component_model_params     | 基于确定的组件和关系创建一个组件匹配模型               | 296  |
| 11   | get_component_model_tree       | 提取组件匹配模型的搜索树                               | 296  |
| 12   | get_component_relations        | 提取组件模型与样品之间的关系                           | 297  |
| 13   | get_found_component_model      | 根据搜索到的目标组件来提取所对应的匹配模型跟成分       | 297  |
| 14   | get_training_components        | 提取一个组件样品模型，根据组件模型和样品图像进行初始化 | 297  |
| 15   | inspect_clustered_components   | 从组件模型中找出刚性的模型组件                         | 298  |
| 16   | modify_component_realtions     | 修改一个样品模型中的关系                               | 298  |
| 17   | read_component_model           | 从一个文件中读取组件匹配模型                           | 298  |
| 18   | read_training_components       | 从一个文件中读取组件模型结果                           | 298  |
| 19   | train_model_components         | 为基于组件模型的匹配对应的组件和范本关系               | 298  |
| 20   | write_component_model          | 把一个组件匹配模型写入一个文件中                       | 299  |
| 21   | write_training_components      | 把一个组件模型写入到一个文件中                         | 299  |

### 15.2 Correlation-Based 相互关系的基本匹配

| 序号 | 函数名                     | 函数说明及注释                                            | 页码 |
| ---- | -------------------------- | --------------------------------------------------------- | ---- |
| 1    | clear_all_ncc_models       | 释放所有NCC（归一化算法，快速匹配）模型的内存             | 299  |
| 2    | clear_ncc_model            | 释放NCC（归一化算法，快速匹配）模型的内存                 | 300  |
| 3    | create_ncc_model           | 创建一个NCC（归一化算法，快速匹配）匹配模型               | 300  |
| 4    | determine_ncc_model_params | 制定NCC（归一化算法，快速匹配）模型参数                   | 300  |
| 5    | find_ncc_model             | 找出图像中的一个NCC（归一化算法，快速匹配）模型的最佳匹配 | 300  |
| 6    | get_ncc_model_origin       | 提取一个NCC（归一化算法，快速匹配）模型的原点（参考点）   | 301  |
| 7    | get_ncc_model_params       | 提取一个NCC（归一化算法，快速匹配）模型的参数             | 301  |
| 8    | read_ncc_model             | 从一个文件中读取一个NCC（归一化算法，快速匹配）模型       | 301  |
| 9    | set_ncc_model_origin       | 设置一个NCC（归一化算法，快速匹配）模型的原点（参考点）   | 301  |
| 10   | set_ncc_model_param        | 设置NCC（归一化算法，快速匹配）模型参数                   | 301  |
| 11   | write_ncc_model            | 向一个文件中保存NCC（归一化算法，快速匹配）模型           | 301  |

### 15.3 Deformable 可变形匹配

| 序号 | 函数名                                     | 函数说明及注释                                            | 页码 |
| ---- | ------------------------------------------ | --------------------------------------------------------- | ---- |
| 1    | clear_all_deformable_models                | 清除所有的可变形模型，释放内存空间                        | 304  |
| 2    | clear_deformable_model                     | 清除指定的可变形模型，释放内存空间                        | 304  |
| 3    | create_local_deformable_model              | 创建一个局部的可变形匹配模型                              | 304  |
| 4    | create_local_deformable_model_xld          | 创建一个局部的可变形XLD匹配模型                           | 305  |
| 5    | create_planar_calib_deformable_model       | 创建一个（带校正透视的）可变形模型                        | 305  |
| 6    | create_planar_calib_deformable_model_xld   | 创建一个以XLD轮廓为平面（带校正透视的）可变形模型         | 306  |
| 7    | create_planar_uncalib_deformable_model     | 创建一个（不带校正透视的）可变形模型                      | 307  |
| 8    | create_planar_uncalib_deformable_model_xld | 创建一个以XLD轮廓为平面（不带校正透视）可变形模型         | 307  |
| 9    | determind_deformable_model_params          | 自动测定一个可变形模型的各项参数及对应值                  | 308  |
| 10   | find_local_deformable_model                | 找出图像中一个局部可变形模型的最佳匹配                    | 308  |
| 11   | find_planar_calib_deformable_model         | 找出图像中一个校正的可变形模型的最佳匹配并返回他的3D姿势  | 309  |
| 12   | find_planar_uncalib_deformable_model       | 找出图像中一个不带校正的可变形模型的最佳匹配              | 310  |
| 13   | get_deformable_model_contours              | 提取一个可变形模型中对应的轮廓                            | 310  |
| 14   | get_deformable_model_origin                | 提取一个可变形模型的原点（参考点）                        | 310  |
| 15   | get_deformable_model_params                | 提取一个可变形模型的参数                                  | 310  |
| 16   | read_deformable_model                      | 从一个文件中读取一个可变形模型                            | 311  |
| 17   | set_deformable_model_origin                | 设置一个可变形模型的原点（参考点）                        | 311  |
| 18   | set_deformable_model_param                 | 设置一个可变形模型的参数                                  | 311  |
| 19   | set_local_deformable_model_metric          | 设置被XLD轮廓产生的可变形模型匹配方法                     | 311  |
| 20   | set_planar_calib_deformable_model_metric   | 设置被XLD轮廓产生的平面（带校正透视）可变形模型匹配方法   | 311  |
| 21   | set_planar_uncalib_deformable_model_metric | 设置被XLD轮廓产生的平面（不带校正透视）可变形模型匹配方法 | 311  |
| 22   | write_deformable_model                     | 将一个可变形模型保存到文件中                              | 312  |

### 15.4 Descriptor-Based 描述符匹配

| 序号 | 函数名                          | 函数说明及注释                             | 页码 |
| ---- | ------------------------------- | ------------------------------------------ | ---- |
| 1    | clear_all_descriptor_models     | 清除所有的描述符匹配模型的内存分配         | 312  |
| 2    | clear_descriptor_model          | 清除一个描述符匹配模型的内存分配           | 312  |
| 3    | create_calib_descriptor_model   | 创建一个校正透视描述符匹配模型             | 312  |
| 4    | create_uncalib_descriptor_model | 准备一个描述符匹配模型                     | 313  |
| 5    | find_calib_descriptor_model     | 在一个图像中寻找最佳校正透视描述符模型     | 313  |
| 6    | find_uncalib_descriptor_model   | 在一个图像中寻找最佳描述符匹配模型         | 314  |
| 7    | get_descriptor_model_origin     | 获取描述符模型的参考点                     | 314  |
| 8    | get_descriptor_model_params     | 获取描述符模型的参数                       | 314  |
| 9    | get_descriptor_model_points     | 获取描述符模型的兴趣点（字符的笔画定位点） | 314  |
| 10   | get_descriptor_model_results    | 获取描述符模型的样品                       | 315  |
| 11   | read_descroptor_model           | 从文件中读取一个描述符模型                 | 315  |
| 12   | set_descriptor_model_origin     | 为一个描述符模型设置参考点                 | 315  |
| 13   | write_descriptor_model          | 将一个描述符模型保存（写入）到文件中       | 315  |

### 15.5 Gray-Value-Based 灰度匹配

| 序号 | 函数名                 | 函数说明及注释                         | 页码 |
| ---- | ---------------------- | -------------------------------------- | ---- |
| 1    | adapt_template         | 把一个模板用于一个图像的大小           | 316  |
| 2    | best_match             | 寻找一个模板和一个图像的最佳匹配       | 316  |
| 3    | best_match_mg          | 在金字塔中寻找最佳灰度值匹配           | 316  |
| 4    | best_match_pre_mg      | 在预生成的金字塔中寻找最佳灰度值匹配   | 316  |
| 5    | best_match_rot         | 寻找一个模板和一个旋转图像的最佳匹配   | 317  |
| 6    | best_match_rot_mg      | 寻找一个模板和一个旋转金字塔的最佳匹配 | 317  |
| 7    | clear_all_templates    | 清除所有模板的内存分配                 | 317  |
| 8    | clear_template         | 清除一个模板的内存分配                 | 317  |
| 9    | create_template        | 为模板匹配准备一个格式                 | 317  |
| 10   | create_template_rot    | 为旋转模板匹配准备一个格式             | 318  |
| 11   | fast_match             | 寻找一个模板和一个图像的最佳匹配       | 318  |
| 12   | fast_match_mg          | 在金字塔中寻找最佳灰度值匹配           | 318  |
| 13   | read_template          | 从一个文件中读取一个模版               | 318  |
| 14   | set_offset_template    | 模板的灰度值偏差                       | 318  |
| 15   | set_reference_template | 为一个匹配模板定义参考位置             | 318  |
| 16   | write_template         | 向一个文件中写入模板                   | 319  |

### 15.6 Shaped-Based 形状匹配

| 序号 | 函数名                             | 函数说明及注释                                       | 页码 |
| ---- | ---------------------------------- | ---------------------------------------------------- | ---- |
| 1    | clear_all_shape_models             | 释放所有轮廓模型的内存                               | 319  |
| 2    | clear_shape_model                  | 释放一个轮廓模型的内存                               | 319  |
| 3    | create_aniso_shape_model           | 准备一个x，y方向可缩放比例的匹配轮廓模型             | 319  |
| 4    | create_aniso_shape_model_xld       | 准备一个x，y方向可缩放比例的匹配XLD轮廓模型          | 320  |
| 5    | create_scaled_shape_model          | 准备一个可缩放比例的匹配轮廓模型                     | 320  |
| 6    | create_scaled_shape_model_xld      | 准备一个可缩放比例的匹配轮廓XLD模型                  | 321  |
| 7    | create_shape_model                 | 准备一个（不可缩放比例的）匹配轮廓模型               | 321  |
| 8    | create_shape_model_xld             | 准备一个不可缩放比例的匹配XLD轮廓模型                | 322  |
| 9    | determine_shape_model_params       | 自动测定一个匹配轮廓模型的各项参数及对应值           | 322  |
| 10   | find_aniso_shape_model             | 在一个图像中找出一个x，y方向可缩放比例的最佳匹配轮廓 | 323  |
| 11   | find_aniso_shape_models            | 在一个图像中找出多个x，y方向可缩放比例的最佳匹配轮廓 | 324  |
| 12   | find_scaled_shape_model            | 在一个图像中找出一个可缩放比例的最佳匹配轮廓         | 326  |
| 13   | find_scaled_shape_models           | 在一个图像中找出多个可缩放比例的最佳匹配轮廓         | 327  |
| 14   | find_shape_model                   | 在一个图像中找出一个（不可缩放比例的）最佳匹配轮廓   | 329  |
| 15   | find_shape_models                  | 在一个图像中找出多个（不可缩放比例的）最佳匹配轮廓   | 330  |
| 16   | get_shape_model_contours           | 返回一个轮廓匹配模型的外形轮廓                       | 332  |
| 17   | get_shape_model_origin             | 返回一个轮廓匹配模型的原点（参考点）                 | 332  |
| 18   | get_shape_model_params             | 返回一个轮廓匹配模型的参数                           | 332  |
| 19   | inspect_shape_model                | 创建一个轮廓匹配模型基于金字塔的图像                 | 332  |
| 20   | read_shape_model                   | 从一个文件中读取一个轮廓匹配模型                     | 332  |
| 21   | set_shape_model_metric             | 设置一个轮廓匹配模型的匹配方法                       | 333  |
| 22   | set_shape_model_origin             | 设置一个轮廓匹配模型的原点（参考点）                 | 333  |
| 23   | set_shape_model_param              | 设置一个轮廓匹配模型的参数                           | 333  |
| 24   | write_shape_model                  | 向一个文件中写入一个轮廓匹配模型                     | 333  |
| 25   | dev_display_shape_matching_results | 显示这个匹配结果                                     | 333  |

## Chapter 16 : Matrix (矩阵)

### 16.1 Access 数据

| 序号 | 函数名              | 函数说明及注释               | 页码 |
| ---- | ------------------- | ---------------------------- | ---- |
| 1    | get_diagonal_matrix | 获取矩阵的对角元素           | 337  |
| 2    | get_full_matrix     | 获取矩阵的所有元素           | 337  |
| 3    | get_sub_matrix      | 获取指定行列的矩阵元祖       | 337  |
| 4    | get_value_matrix    | 获取矩阵的所有元素值转为元祖 | 338  |
| 5    | set_diagonal_matrix | 设置矩阵的对角元素           | 338  |
| 6    | set_full_matrix     | 设置矩阵的所有元素           | 338  |
| 7    | set_sub_matrix      | 设置指定行列的矩阵元祖       | 338  |
| 8    | set_value_matrix    | 设置指定行列的矩阵元祖       | 339  |

### 16.2 Arithmetic 计算

| 序号 | 函数名                        | 函数说明及注释                                 | 页码 |
| ---- | ----------------------------- | ---------------------------------------------- | ---- |
| 1    | abs_matrix                    | 计算矩阵元素的绝对值，产生一个新的矩阵         | 340  |
| 2    | abs_matrix_mod                | 对矩阵自身进行绝对值运算                       | 340  |
| 3    | add_matrix                    | 两矩阵进行相加操作，产生一个新的矩阵           | 340  |
| 4    | add_matrix_mod                | 两矩阵进行相加操作，并覆盖第一矩阵             | 340  |
| 5    | div_element_matrix            | 两矩阵进行相除操作，产生一个新的矩阵           | 340  |
| 6    | div_element_matrix_mod        | 两矩阵进行相除操作，并覆盖第一矩阵             | 341  |
| 7    | invert_matrix                 | 逆矩阵运算                                     | 341  |
| 8    | invert_matrix_mod             | 逆矩阵运算                                     | 341  |
| 9    | mult_element_matrix           | 两矩阵相乘操作，产生一个新的矩阵               | 341  |
| 10   | mult_element_matrix_mod       | 两矩阵进行相乘操作，计算返回值覆盖该矩阵       | 342  |
| 11   | mult_matrix                   | 矩阵乘法运算                                   | 342  |
| 12   | mult_matrix_mod               | 矩阵乘法运算，计算返回值覆盖该矩阵             | 342  |
| 13   | pow_element_matrix            | 计算一个矩阵元素的幂运算                       | 342  |
| 14   | pow_element_matrix_mod        | 计算一个矩阵元素的幂运算，计算返回值覆盖该矩阵 | 342  |
| 15   | pow_matrix                    | 矩阵的幂运算操作，产生一个新的矩阵             | 343  |
| 16   | pow_matrix_mod                | 计算一个矩阵元素的幂运算，计算返回值覆盖该矩阵 | 343  |
| 17   | pow_scalar_element_matrix     | 矩阵的乘方运算操作，产生一个新的矩阵           | 343  |
| 18   | pow_scalar_element_matrix_mod | 矩阵的乘方运算操作，计算返回值覆盖该矩阵       | 343  |
| 19   | scale_matrix                  | 矩阵比例缩放操作，产生一个新的矩阵             | 343  |
| 20   | scale_matrix_mod              | 矩阵比例缩放操作，计算返回值覆盖该矩阵         | 344  |
| 21   | solve_matrix                  | 计算解答方程组                                 | 344  |
| 22   | sqrt_matrix                   | 矩阵的根方操作，产生一个新的矩阵               | 344  |
| 23   | sqrt_matrix                   | 矩阵的根方操作，计算返回值覆盖该矩阵           | 344  |
| 24   | sub_matrix                    | 矩阵的减法操作，产生一个新的矩阵               | 344  |
| 25   | sub_matrix_mod                | 矩阵的减法操作，计算返回值覆盖该矩阵           | 345  |
| 26   | transpose_matrix              | 矩阵位置变换，产生一个新的矩阵                 | 345  |
| 27   | transpose_matrix_mod          | 矩阵位置变换，计算返回值覆盖该矩阵             | 345  |

### 3416.3 Creation 创建

| 序号 | 函数名             | 函数说明及注释                                             | 页码 |
| ---- | ------------------ | ---------------------------------------------------------- | ---- |
| 1    | clear_all_matrices | 清除所有的矩阵，该函数不建议操作，将可能导致不可预料的后果 | 345  |
| 2    | clear_matrix       | 清除指定矩阵                                               | 345  |
| 3    | copy_matrix        | 复制一个矩阵                                               | 345  |
| 4    | create_matrix      | 创建一个矩阵                                               | 346  |
| 5    | repeat_matrix      | 产生一个排列矩阵（该矩阵按设置倍数进行排列一个矩阵）       | 346  |

### 16.4 Decomposition 分解

| 序号 | 函数名                      | 函数说明及注释     | 页码 |
| ---- | --------------------------- | ------------------ | ---- |
| 1    | decompose_matrix            | 分解一个矩阵       | 346  |
| 2    | orthogonal_decompose_matrix | 正交分解一个矩阵   | 347  |
| 3    | svd_matrix                  | 计算奇异值分解矩阵 | 347  |

### 16.5 Eigenvalues 特征值

| 序号 | 函数名                                   | 函数说明及注释                         | 页码 |
| ---- | ---------------------------------------- | -------------------------------------- | ---- |
| 1    | eigenvalues_general_matrix               | 计算一个普通矩阵的本征值和特征向量     | 347  |
| 2    | eigenvalues_symmetric_matrix             | 计算一个对称矩阵的本征值和特征向量     | 347  |
| 3    | generalized_elgenvalues_general_matrix   | 计算一个普通矩阵的广义本征值和特征向量 | 347  |
| 4    | generalized_elgenvalues_symmetric_matrix | 计算一个对称矩阵的广义本征值和特征向量 | 348  |

### 16.6 Features 特征

| 序号 | 函数名             | 函数说明及注释     | 页码 |
| ---- | ------------------ | ------------------ | ---- |
| 1    | determinant_matrix | 计算矩阵的决定因素 | 348  |
| 2    | get_size_matrix    | 计算矩阵的元素数量 | 348  |
| 3    | max_matrix         | 计算矩阵的最大值   | 348  |
| 4    | mean_matrix        | 计算矩阵的平均值   | 349  |
| 5    | min_matrix         | 计算矩阵的最小值   | 349  |
| 6    | norm_matrix        | 矩阵标准值         | 349  |
| 7    | sum_matrix         | 返回矩阵的阵列     | 349  |

### 16.7 File文件

| 序号 | 函数名       | 函数说明及注释     | 页码 |
| ---- | ------------ | ------------------ | ---- |
| 1    | read_matrix  | 读取矩阵文件       | 350  |
| 2    | write_matrix | 把矩阵写入到文件中 | 350  |

## Chapter 17: Morpholopy （形态学）

### 17.1 Gray-Values 灰度值

| 序号 | 函数名              | 函数说明及注释                         | 页码 |
| ---- | ------------------- | -------------------------------------- | ---- |
| 1    | dual_rank           | 打开、取中值和关闭圆和矩形掩码         | 353  |
| 2    | gen_disc_se         | 为灰度形态学生成椭圆结构基础           | 354  |
| 3    | gray_bothat         | 执行一个图像的一个灰度值bottom_hat变换 | 354  |
| 4    | gray_closing        | 关闭一个图像的一个灰度值               | 355  |
| 5    | gray_closing_rect   | 关闭带矩形掩码的灰度值                 | 355  |
| 6    | gray_closing_shape  | 关闭带选择掩码的灰度值                 | 355  |
| 7    | gray_dilation       | 膨胀一个图像的灰度值                   | 356  |
| 8    | gray_dilation_rect  | 确定一个矩形的最大灰度值               | 357  |
| 9    | gray_dilation_shape | 确定一个选择的掩码的最大灰度值         | 357  |
| 10   | gray_erosion        | 腐蚀一个图像的灰度值                   | 357  |
| 11   | gray_erosion_rect   | 确定一个矩形的最小灰度值               | 358  |
| 12   | gray_erosion_shape  | 确定一个选择的掩码的最小灰度值         | 358  |
| 13   | gray_opening        | 打开一个图像的灰度值                   | 358  |
| 14   | gray_opening_rect   | 打开一个矩形掩码的灰度值               | 359  |
| 15   | gray_opening_shape  | 打开一个选择的掩码的灰度值             | 359  |
| 16   | gray_range_rect     | 确定一个矩形的灰度值范围               | 359  |
| 17   | gray_tophat         | 执行一个图像的一个灰度值top_hat变换    | 360  |
| 18   | read_gray_se        | 为灰度形态学下载一个结构基础           | 360  |

### 17.2 Region 区域

| 序号 | 函数名              | 函数说明及注释                                               | 页码 |
| ---- | ------------------- | ------------------------------------------------------------ | ---- |
| 1    | bottom_hat          | 修补区域的外围，以制定的区域类修补                           | 361  |
| 2    | boundary            | 把一个区域减小到它的边界                                     | 362  |
| 3    | closing             | 闭运算一个成分区域结构的修正区域                             | 362  |
| 4    | closing_circle      | 闭运算一个圆形结构基础的修正区域                             | 363  |
| 5    | closing_golay       | 闭运算格雷字母表中的元素的一个区域                           | 364  |
| 6    | closing_rectangle1  | 闭运算一个矩形结构基础的修正区域                             | 364  |
| 7    | dilation1           | 膨胀一个区域                                                 | 364  |
| 8    | dialtion2           | 膨胀一个区域（使用一个参考点）                               | 365  |
| 9    | dilation_circle     | 膨胀一个圆形结构基础的一个区域                               | 366  |
| 10   | dilation_golay      | 膨胀格雷字母表中的元素的一个区域                             | 367  |
| 11   | dilation_rectangle1 | 膨胀一个矩形结构基础的一个区域                               | 367  |
| 12   | dilation_seg        | 顺序膨胀一个区域                                             | 367  |
| 13   | erosion1            | 腐蚀一个区域                                                 | 367  |
| 14   | erosion2            | 腐蚀一个区域（使用一个参考点）                               | 367  |
| 15   | erosion_circle      | 腐蚀一个圆形结构基础的一个区域                               | 368  |
| 16   | erosion_golay       | 腐蚀格雷字母表的一个元素的一个区域                           | 368  |
| 17   | erosion_rectangle1  | 腐蚀一个矩形结构基础的一个区域                               | 368  |
| 18   | erosion_seq         | 顺序腐蚀一个区域                                             | 368  |
| 19   | fitting             | 执行多重结构基础的打开后关闭                                 | 368  |
| 20   | gen_struct_elements | 生成一个标准结构基础                                         | 369  |
| 21   | golay_elements      | 生成格雷字母表的结构基础                                     | 369  |
| 22   | hit_or_miss         | 使一个区域通过指定构成元素进行边影区域提取操作               | 370  |
| 23   | hit_or_miss_golay   | 使用格雷字母表的区域的边影区域提取操作                       | 370  |
| 24   | hit_or_miss_seq     | 使用格雷字母表的区域按顺序整体进行边影区域提取               | 371  |
| 25   | minkowski_add1      | 用一种修补区域来膨胀另一个区域                               | 371  |
| 26   | minkowski_add2      | 用一种修补区域来膨胀另一个区域（使用参考点）                 | 372  |
| 27   | minkowski_sub1      | 用一种修补区域来腐蚀另一个区域                               | 372  |
| 28   | minkowski_sub2      | 用一种修补区域来腐蚀另一个区域（使用参考点）                 | 373  |
| 29   | morph_hat           | 计算bottom_hat和top_hat的联合                                | 373  |
| 30   | morph_skeleton      | 计算一个区域的形态学框架                                     | 374  |
| 31   | morph_skiz          | 缩小一个区域                                                 | 374  |
| 32   | opening             | 开运算一个被提取了成分的区域                                 | 375  |
| 33   | opening_circle      | 开运算一个圆形结构基础的一个区域                             | 376  |
| 34   | opening_golay       | 开运算格雷字母表的一个元素的一个区域                         | 376  |
| 35   | opening_rectangle1  | 开运算一个矩形结构基础的一个区域                             | 376  |
| 36   | opening_seq         | 分离重叠区域                                                 | 377  |
| 37   | pruning             | 去掉一个区域的分支                                           | 377  |
| 38   | thickening          | 使一个区域通过Rolay构成元素进行加厚操作                      | 377  |
| 39   | thickening_golay    | 使一个区域通过Rolay构成元素进行加厚操作（使用一个Golay结构基础） | 378  |
| 40   | thickening_seq      | 使一个区域通过Rolay构成元素进行加厚操作（按顺序）            | 378  |
| 41   | thinning            | 使一个区域通过指定构成元素进行变薄操作（按参考点）           | 378  |
| 42   | thinning_golay      | 使一个区域通过Rolay构成元素进行变薄操作                      | 379  |
| 43   | thinning_seq        | 使一个区域通过Rolay构成元素进行变薄操作（按顺序）            | 379  |
| 44   | top_hat             | 计算区域的top_hat（原图像和它的开运算之间的差）              | 380  |

## Chapter 18: OCR （光学字符识别）

### 18.1 Hyperboxes

| 序号 | 函数名               | 函数说明及注释                                            | 页码 |
| ---- | -------------------- | --------------------------------------------------------- | ---- |
| 1    | close_all_ocrs       | 删除所有OCR句柄模型，释放存储空间，但会丢失所有的测试数据 | 385  |
| 2    | close_ocr            | 删除一个OCR句柄模型，对应的测试数据将会丢失               | 385  |
| 3    | create_ocr_class_box | 创建新的OCR分级器                                         | 385  |
| 4    | do_ocr_multi         | 给每一个字符分配一个类                                    | 385  |
| 5    | do_ocr_single        | 识别一个字符                                              | 386  |
| 6    | info_ocr_class_box   | 反馈OCR的有关信息                                         | 386  |
| 7    | ocr_change_char      | 为字符建立新的查阅表                                      | 386  |
| 8    | ocr_get_features     | 计算给定字符的特征参数                                    | 386  |
| 9    | read_ocr             | 从文件中读取OCR分级器                                     | 386  |
| 10   | testd_ocr_class_box  | 测试给定类中字符的置信度                                  | 386  |
| 11   | traind_ocr_class_box | 通过一副图像的特定区域直接测试分级器                      | 386  |
| 12   | trainf_ocr_class_box | 根据指定测试文件测试分级器的OCRHandle                     | 387  |
| 13   | write_ocr            | 将OCR分级器的OCRHandle写入文件的文件名                    | 387  |

### 18.2 Lexica 词典

| 序号 | 函数名           | 函数说明及注释                                               | 页码 |
| ---- | ---------------- | ------------------------------------------------------------ | ---- |
| 1    | clear_all_lexica | 清除所有的词汇（词典），释放它们的资源                       | 388  |
| 2    | clear_lexicon    | 清除一个词汇（词典），释放相应的资源                         | 388  |
| 3    | create_lexicon   | 创建一个新的单词列表，输出该词典句柄                         | 388  |
| 4    | import_lexicon   | 通过文件名选定的文件中的一系列单词创建一个新的词典           | 388  |
| 5    | inspect_lexicon  | 返回对应参数的词典中所有单词的元祖                           | 388  |
| 6    | lookup_lexicon   | 检查单词是否在词典的LexiconHandle中，若在返回1否则返回0      | 388  |
| 7    | suggest_lexicon  | 对单词与所有词汇比较，输出最相似的词汇，给出单个字符错别数量 | 388  |

### 18.3 Neural-Nets 神经网络

| 序号 | 函数名                      | 函数说明及注释                                               | 页码 |
| ---- | --------------------------- | ------------------------------------------------------------ | ---- |
| 1    | clear_all_ocr_class_mlp     | 清除所有创建的OCR分类器，释放分类占据的存储空间              | 389  |
| 2    | clear_ocr_class_mlp         | 清除一个创建的OCR分类器，释放该分类器占据的存储空间          | 389  |
| 3    | create_ocr_class_mlp        | 利用MLP（多层感知器）创建一个新的OCR分级器                   | 389  |
| 4    | do_ocr_multi_class_mlp      | 对一组字符区域内容进行识别，输出到Class中去                  | 390  |
| 5    | do_ocr_single_class_mlp     | 对单个字符区域内容进行识别，按多个匹配字符输出到Class中去    | 390  |
| 6    | do_ocr_word_mlp             | 对一个词汇字符区域内容进行OCR_mlp模型识别，单字符输出到Class，词汇输出到Word中 | 392  |
| 7    | get_features_ocr_class_mlp  | 根据OCRHandle确定的字符计算其特征参数，并将它们返回          | 393  |
| 8    | get_params_ocr_class_mlp    | 返回一个OCR_mlp模型对应的各项参数                            | 393  |
| 9    | get_prep_info_ocr_class_mlp | 计算OCR分级器预设定矢量特性的信息                            | 393  |
| 10   | read_ocr_class_mlp          | 从一个文件中读取OCR分级器                                    | 393  |
| 11   | trainf_ocr_class_mlp        | 测试OCRHandle，根据存储在OCR文件中的测试特性                 | 394  |
| 12   | write_ocr_class_mlp         | 将OCR分级器的OCRHandle写入由文件名确定的文件中               | 394  |

### 18.4 Segmentation 分割

| 序号 | 函数名                 | 函数说明及注释                                         | 页码 |
| ---- | ---------------------- | ------------------------------------------------------ | ---- |
| 1    | clear_all_text_models  | 清除所有的文字模型，释放内存                           | 395  |
| 2    | clear_all_text_results | 清除所有的文字搜索结果                                 | 395  |
| 3    | clear_text_model       | 清除一个文字模型，释放内存                             | 395  |
| 4    | clear_text_result      | 创建一个文字模版                                       | 395  |
| 5    | create_text_model      | 创建一个文字模版                                       | 395  |
| 6    | find_text              | 在图像中查找文字片段                                   | 396  |
| 7    | get_text_model_param   | 查找文字模型参数                                       | 396  |
| 8    | get_text_object        | 从文本分割片段中提取对应区域数组ResultName中一个片段域 | 396  |
| 9    | get_text_result        | 从中提取被分割出来的文本片段，并保留到ResultName中     | 396  |
| 10   | segment_characters     | 将一副图像给定区域的字符分割                           | 396  |
| 11   | select_characters      | 从一个给定字符区域中分离字符（区域数组）               | 397  |
| 12   | set_text_model_param   | 设置文字模型参数                                       | 398  |
| 13   | text_line_orientation  | 提取图像中一个文本行或段落的定向（旋转方向）           | 398  |
| 14   | text_line_slant        | 提取图像中一个文本行或段落对应字符的倾斜角度           | 399  |

### 18.5 Support-Vertor-Machines 支持向量机

| 序号 | 函数名                               | 函数说明及注释                                      | 页码 |
| ---- | ------------------------------------ | --------------------------------------------------- | ---- |
| 1    | clear_all_ocr_class_svm              | 清除所有的基于OCR分级器的SVM，释放相应的存储空间    | 400  |
| 2    | clear_ocr_class_svm                  | 清除基于OCR分级器的一个SVM，释放相应的存储空间      | 400  |
| 3    | create_ocr_class_svm                 | 利用支持向量机创建一个OCR分级器                     | 400  |
| 4    | do_ocr_multi_class_svm               | 根据基于OCR分级器的SVM将大量字符分类                | 400  |
| 5    | do_ocr_single_class_svm              | 根据基于OCR分级器的SVM将单个字符分类                | 401  |
| 6    | do_ocr_word_svm                      | 利用OCR分级器将一系列相关字符分类                   | 401  |
| 7    | get_features_ocr_class_svm           | 计算一个字符的特征                                  | 401  |
| 8    | get_params_ocr_class_svm             | 返回一个OCR分级器的参数                             | 401  |
| 9    | get_prep_info_ocr_class_svm          | 计算基于OCR分级器的SVM的预定义特征矢量的信息内容    | 402  |
| 10   | get_support_vector_num_ocr_class_svm | 返回OCR分级器支持的矢量的数目                       | 402  |
| 11   | get_support_vector_ocr_class_svm     | 返回基于支持向量机的已测试OCR分级器中支持向量的索引 | 402  |
| 12   | read_ocr_class_svm                   | 从文件中读取基于OCR分级器的SVM                      | 402  |
| 13   | reduce_ocr_class_svm                 | 根据一个减小的SVM来接近一个基于OCR分级器的SVM       | 402  |
| 14   | trainf_ocr_class_svm                 | 测试一个OCR分级器                                   | 402  |
| 15   | write_ocr_class_svm                  | 将一个OCR分级器 写入文件                            | 403  |

### 18.6 Training-Files 测试夹

| 序号 | 函数名                 | 函数说明及注释                             | 页码 |
| ---- | ---------------------- | ------------------------------------------ | ---- |
| 1    | append_ocr_trainf      | 将字符添加到一个测试文件中                 | 403  |
| 2    | concat_ocr_trainf      | 合并测试文件                               | 403  |
| 3    | read_ocr_trainf        | 从文件中读取字符，将其转换到图像中         | 403  |
| 4    | read_ocr_trainf_names  | 查询哪些字符存储在测试文件中               | 403  |
| 5    | read_ocr_trainf_select | 从文件中读取测试特定字符，将其转换到图像中 | 403  |
| 6    | write_ocr_trainf       | 将已测试的字符存储到文件中                 | 404  |
| 7    | write_ocr_trainf_image | 将字符写入正在测试的文件中                 | 404  |

## Chapter 19: Object（对象、目标）

### 19.1 Information 消息

| 序号 | 函数名           | 函数说明及注释             | 页码 |
| ---- | ---------------- | -------------------------- | ---- |
| 1    | count_obj        | 统计一个元祖中的对象       | 407  |
| 2    | get_channel_info | 一幅目标图像组成部分的信息 | 407  |
| 3    | get_object_class | 一幅目标图像类的名称       | 407  |
| 4    | test_equal_obj   | 比较目标图像是否相等       | 408  |

### 19.2 Manipulation 纂改

| 序号 | 函数名         | 函数说明及注释                     | 页码 |
| ---- | -------------- | ---------------------------------- | ---- |
| 1    | clear_obj      | 将一个目标元祖从HALCON数据库中删除 | 408  |
| 2    | concat_obj     | 连接两个目标元祖的图标             | 409  |
| 3    | copy_obj       | 复制一个目标元祖对象               | 409  |
| 4    | gen_empty_obj  | 创建一个空的目标元祖               | 410  |
| 5    | integer_to_obj | 将一个整型数转换为一个图标         | 410  |
| 6    | obj_diff       | 计算两个目标元祖之间的差异         | 410  |
| 7    | obj_to_integer | 将一个图标转换为一个整型数         | 411  |
| 8    | select_obj     | 复制一个目标选择的索引部分         | 411  |

## Chapter 20: Regions（区域）

### 20.1 Access 数据

| 序号 | 函数名             | 函数说明及注释                       | 页码 |
| ---- | ------------------ | ------------------------------------ | ---- |
| 1    | get_region_chain   | 一个对象的轮廓作为链式码             | 415  |
| 2    | get_region_contour | 获取一个区域的外围轮廓，各个点的坐标 | 415  |
| 3    | get_region_convex  | 查询突起的外表作为轮廓               | 416  |
| 4    | get_region_points  | 查询一个区域的像素点                 | 416  |
| 5    | get_region_polygon | 获取一个区域的近似多边形             | 417  |
| 6    | get_region_runs    | 查询一个区域的扫描宽度编码           | 418  |

### 20.2 Creation 创建区域

| 序号 | 函数名                    | 函数说明及注释                          | 页码 |
| ---- | ------------------------- | --------------------------------------- | ---- |
| 1    | gen_checker_region        | 创建一个方格式区域                      | 420  |
| 2    | gen_circle                | 创建一个圆周                            | 420  |
| 3    | gen_ellipse               | 创建一个椭圆                            | 420  |
| 4    | gen_empty_region          | 创建一个空的区域                        | 421  |
| 5    | gen_grid_region           | 创建一个网格区域                        | 421  |
| 6    | gen_random_region         | 创建一个随机区域                        | 421  |
| 7    | gen_random_regions        | 创建随机区域如圆周，矩形和椭圆          | 422  |
| 8    | gen_rectangle1            | 创建一个与坐标轴平行的长方形            | 422  |
| 9    | gen_rectangle2            | 创建任意方向的矩形                      | 422  |
| 10   | gen_region_contour_xld    | 从XLD元祖中创建一个区域                 | 423  |
| 11   | gen_region_histo          | 将一个直方图转换为一个区域              | 423  |
| 12   | gen_region_hline          | 将Hesse正规形状中描述的输入线存储为区域 | 423  |
| 13   | gen_region_line           | 将输入线以区域形式存储                  | 423  |
| 14   | gen_region_points         | 将个别的像素存储为图像区域              | 423  |
| 15   | gen_region_polygon        | 将一个多边形存储为一个目标图像          | 423  |
| 16   | gen_region_polygon_filled | 将一个多边形存储为一个已填充区域        | 423  |
| 17   | gen_region_polygon_xld    | 创建一个XLD多边形中的区域               | 424  |
| 18   | gen_region_runs           | 创建一个扫描宽度编码中的图像区域        | 424  |
| 19   | label_to_regions          | 提取一幅图像中灰度值相同的区域          | 424  |

### 20.3 Features 特征

| 序号 | 函数名                       | 函数说明及注释                                               | 页码 |
| ---- | ---------------------------- | ------------------------------------------------------------ | ---- |
| 1    | area_center                  | 提取一个区域的面积（大小）和中心                             | 426  |
| 2    | area_holes                   | 提取一个区域中洞（封闭的裂缝）的面积                         | 426  |
| 3    | circularity                  | 提取一个区域与圆的相似度的形状系数                           | 427  |
| 4    | compactness                  | 提取一个区域致密度的形状系数                                 | 427  |
| 5    | connect_and_holes            | 提取区域中组成部分的数量及该区域中孔的数目                   | 428  |
| 6    | contlength                   | 提取一个区域轮廓（contour）的长度                            | 429  |
| 7    | convexity                    | 提取一个区域凸性的形状系数                                   | 429  |
| 8    | diameter_region              | 提取一个区域中最大的直线距离                                 | 429  |
| 9    | eccentricity                 | 提取一个类似椭圆的形状系数                                   | 430  |
| 10   | elliptic_axis                | 提取一个区域中等值（类似于）椭圆的参数                       | 430  |
| 11   | euler_number                 | 计算区域中存在的区域总数与孔（洞）的数量差异                 | 431  |
| 12   | find_neighbors               | 提取一个区域的最大距离内的邻域                               | 431  |
| 13   | get_region_index             | 查找指定位置所在区域的索引值                                 | 431  |
| 14   | get_region_thickness         | 查询主轴附近区域的宽度（厚度）                               | 432  |
| 15   | hamming_distance             | 两个区域间的汉明距离                                         | 432  |
| 16   | hamming_distance_norm        | 两个区域间的归一化汉明距离                                   | 433  |
| 17   | inner_circle                 | 提取一个区域内部最大的外切圆                                 | 433  |
| 18   | inner_rectangle1             | 提取一个区域内部最大的矩形                                   | 433  |
| 19   | moments_region_2nd           | 区域的某时刻几何特性                                         | 434  |
| 20   | moments_region_2nd_invar     | 区域的某时刻几何特性                                         | 434  |
| 21   | moments_region_2nd_rel_invar | 计算相关时刻参数                                             | 434  |
| 22   | moments_region_3rd           | 区域的某时刻几何特性                                         | 434  |
| 23   | moments_region_3nd_invar     | 区域的某时刻几何特性                                         | 434  |
| 24   | moments_region_central       | 区域的某时刻几何特性                                         | 435  |
| 25   | moments_region_central_invar | 区域的某时刻几何特性                                         | 435  |
| 26   | orientation_region           | 提取一个区域的定向                                           | 435  |
| 27   | rectangularity               | 提取一个区域对应矩形（长方形）相似程度的形状系数             | 436  |
| 28   | roundness                    | 提取一个区域轮廓的形状系数                                   | 437  |
| 29   | runlength_distribution       | 一个区域扫描宽度编码所需的顺串的分配                         | 437  |
| 30   | runlength_features           | 区域扫描宽度编码的特征值                                     | 438  |
| 31   | select_region_point          | 选择包括给定像素在内的所有区域                               | 438  |
| 32   | select_region_spatial        | 根据区域关联提取周边（上、下、左、右）的区域                 | 438  |
| 33   | select_shape                 | 根据区域要求的特征提取适应的区域                             | 439  |
| 34   | select_shape_proto           | 选择彼此由某种关系的区域                                     | 440  |
| 35   | select_shape_std             | 根据给定形状特征提取适应的区域                               | 440  |
| 36   | smallest_circle              | 提取一区域的最小半径                                         | 441  |
| 37   | smallest_rectangle1          | 提取包围某区域的最小水平矩形                                 | 441  |
| 38   | smallest_rectangle2          | 提取包围某区域的最小任意矩形                                 | 442  |
| 39   | spatial_relation             | 对比一个区域判断其它区域在该区域的哪个方位（上、下、左、右） | 442  |
| 40   | get_features                 | 提取特征区域和圆                                             | 443  |

### 20.4 Geometric-Transformations 几何变换

| 序号 | 函数名                  | 函数说明及注释                             | 页码 |
| ---- | ----------------------- | ------------------------------------------ | ---- |
| 1    | affine_trans_region     | 对区域进行任意的二维变换                   | 444  |
| 2    | mirror_region           | 对区域进行镜像变换                         | 444  |
| 3    | move_region             | 对区域进行水平垂直方向移动                 | 445  |
| 4    | polar_trans_region      | 将一个环状弧内的区域转换为极坐标           | 446  |
| 5    | polar_trans_region_inv  | 将极坐标中的区域转换为笛卡尔坐标系中的区域 | 446  |
| 6    | projective_trans_region | 对一个区域进行射影变换                     | 448  |
| 7    | transpose_region        | 对一个区域以某个点进行旋转                 | 448  |
| 8    | zoom_region             | 缩放一个区域                               | 448  |

### 20.5 Sets 集合

| 序号 | 函数名          | 函数说明及注释                                             | 页码 |
| ---- | --------------- | ---------------------------------------------------------- | ---- |
| 1    | complement      | 返回一个区域的补集（补码），用窗口全部区域减去该区域的差集 | 449  |
| 2    | difference      | 计算两个区域的差集，第1区域预留部分形成新区域              | 450  |
| 3    | intersection    | 计算两个区域的交集                                         | 450  |
| 4    | symm_difference | 计算两个区域对称差异                                       | 451  |
| 5    | union1          | 返回所有输入区域的并集                                     | 451  |
| 6    | union2          | 返回两个区域的并集                                         | 451  |

### 20.6 Tests 测试

| 序号 | 函数名             | 函数说明及注释                     | 页码 |
| ---- | ------------------ | ---------------------------------- | ---- |
| 1    | test_equal_region  | 检测两个目标区域是否相同           | 452  |
| 2    | test_region_poing  | 检测一个测试点是否在区域内         | 453  |
| 3    | rest_subset_region | 检测一个区域是否包含在两一个区域中 | 453  |

### 20.7 Transformation 变换

| 序号 | 函数名                  | 函数说明及注释                       | 页码 |
| ---- | ----------------------- | ------------------------------------ | ---- |
| 1    | background_seq          | 决定给定区域背景相连的部分           | 453  |
| 2    | clip_region             | 将一个区域修改为矩形                 | 454  |
| 3    | clip_region_rel         | 根据大小修改一个区域                 | 454  |
| 4    | closest_point_transform | 计算这个区域中距离变换的闭点         | 455  |
| 5    | connection              | 计算一个区域相连接的部分             | 455  |
| 6    | distance_transform      | 计算一个区域的距离变换               | 456  |
| 7    | eliminate_runs          | 消除一个给定宽度的顺串               | 457  |
| 8    | expand_region           | 填充区域间的间隙或分离互相重叠区域   | 457  |
| 9    | fill_up                 | 填充区域中的孔，裂缝等               | 458  |
| 10   | fill_up_shape           | 填充拥有给定图形特征区域的中断       | 458  |
| 11   | hamming_change_region   | 创建一个有给定汉明距离的区域         | 459  |
| 12   | interjacent             | 利用给定区域分割图像                 | 460  |
| 13   | junctions_skeleton      | 找出框架中的结点和终点               | 460  |
| 14   | merge_regions_line_scan | 从行扫描图像合并区域                 | 461  |
| 15   | partition_dynamic       | 在较小垂直范围的位置水平分割一个区域 | 461  |
| 16   | partition_rectangle     | 将一个区域分割为等大的矩形           | 462  |
| 17   | rank_region             | 给对区域的大小进行归类               | 462  |
| 18   | remove_noise_region     | 去除一个区域内的噪声                 | 463  |
| 19   | shape_trans             | 改变一个区域的形状                   | 463  |
| 20   | skeleton                | 计算一个区域的框架                   | 463  |
| 21   | sort_region             | 根据相邻位置归类区域                 | 464  |
| 22   | split_skeleton_lines    | 用一个像素宽，没有分支的线来分离线   | 465  |
| 23   | split_skeleton_region   | 用一个像素宽，没有分支的区域来分离线 | 466  |

## Chapter 21: Segmentation（分割）

### 21.1 Classification 类别分割

| 序号 | 函数名                      | 函数说明及注释                                               | 页码 |
| ---- | --------------------------- | ------------------------------------------------------------ | ---- |
| 1    | add_samples_image_class_gmm | 将从图像中获取的测试样本添加到高斯混合模型的测试数据库中     | 469  |
| 2    | add_samples_image_class_mlp | 将从图像中获取的测试样本添加到多层感知器模型的测试数据库中   | 469  |
| 3    | add_samples_image_class_svm | 将从图像中获取的测试样本添加到一个支持向量机模型的测试数据库中 | 469  |
| 4    | class_2dim_sup              | 采用二维空间像素分类分割图像                                 | 469  |
| 5    | class_2dim_unsup            | 将两幅图像以聚类分割                                         | 470  |
| 6    | class_ndim_box              | 利用立方体将像素分类                                         | 470  |
| 7    | class_ndim_borm             | 利用球体或立方体将像素分类                                   | 471  |
| 8    | classify_image_class_gmm    | 根据高斯混合模式分类图像                                     | 472  |
| 9    | classify_image_class_lut    | 根据颜色查找表模式分类图像                                   | 472  |
| 10   | classify_image_class_mlp    | 根据多层感知器分类图像                                       | 474  |
| 11   | classify_image_class_svm    | 根据支持向量机分类图像                                       | 475  |
| 12   | learn_ndim_box              | 利用多通道图像测试一个分级器                                 | 476  |
| 13   | learn_ndim_norm             | 为class_ndim_norm构建类                                      | 476  |

### 21.2 Edges 边界分割

| 序号 | 函数名                 | 函数说明及注释                         | 页码 |
| ---- | ---------------------- | -------------------------------------- | ---- |
| 1    | detect_edge_segments   | 图像中检测直线边缘分割                 | 476  |
| 2    | hysteresis_threshold   | 对一副图像采取磁滞门限进行分割         | 477  |
| 3    | nonmax_suppression_amp | 抑制一幅图像上的非最大值点             | 477  |
| 4    | nonmax_suppression_dir | 利用指定图像抑制一幅图像上的非最大值点 | 478  |

### 21.3 Regiongrowing 区域分割

| 序号 | 函数名             | 函数说明及注释                                   | 页码 |
| ---- | ------------------ | ------------------------------------------------ | ---- |
| 1    | expand_gray        | 依据灰度值或颜色填充两个区域的间隙或分割重叠区域 | 478  |
| 2    | expand_gray_ref    | 依据灰度值或颜色填充两个区域的间隙或分割重叠区域 | 479  |
| 3    | expand_line        | 从给定线开始扩充区域                             | 479  |
| 4    | regiongrowing      | 利用区域增长分割图像                             | 480  |
| 5    | regiongrowing_mean | 利用平均灰度值执行区域增长                       | 481  |
| 6    | regiongrowing_n    | 利用区域增长为多通道图像分割图像                 | 482  |

### 21.4 Threshold 门槛值分割

| 序号 | 函数名                | 函数说明及注释                                       | 页码 |
| ---- | --------------------- | ---------------------------------------------------- | ---- |
| 1    | auto_threshold        | 根据直方图决定的阀值分割图像                         | 483  |
| 2    | bin_threshold         | 根据自动产生的阀值分割图像                           | 483  |
| 3    | char_threshold        | 为提取的字符产生一个分割图像                         | 484  |
| 4    | check_threshold       | 一个像素一个像素的比较两幅图像                       | 484  |
| 5    | dual_threshold        | 对指定的图像作门限操作                               | 485  |
| 6    | dyn_threshold         | 利用局部阀值（区域的明亮或黑暗）分割图像             | 485  |
| 7    | fast_threshold        | 利用全局阀值快速将图像二值化                         | 486  |
| 8    | histo_to_thresh       | 根据直方图决定灰度值门限                             | 487  |
| 9    | threshold             | 利用全局阀值分割图像                                 | 487  |
| 10   | threshold_sub_pix     | 根据子像素的标准性从一副图像中提取水平（平坦）交叉口 | 488  |
| 11   | var_threshold         | 根据局域平均标注偏差分析将图像二值化                 | 488  |
| 12   | zero_crossing         | 从一幅图像中提取零相交                               | 489  |
| 13   | zero_crossing_sub_pix | 根据子像素准确性从一幅图像中提取零相交               | 489  |

### 21.5 Topography 灰度分割

| 序号 | 函数名                  | 函数说明及注释                         | 页码 |
| ---- | ----------------------- | -------------------------------------- | ---- |
| 1    | critical_points_sub_pix | 对一幅图像中的鞍点进行精确检测         | 490  |
| 2    | local_max               | 检测一幅图像中所有的最大数             | 491  |
| 3    | local_max_sub_pix       | 一幅图像中局域最大数的子像素精确度检测 | 491  |
| 4    | local_min               | 检测一幅图像中所有的最小数             | 492  |
| 5    | local_min_sub_pix       | 一幅图像中局域最小数的子像素精确度检测 | 493  |
| 6    | lowlands                | 检测凹地所有灰度值                     | 493  |
| 7    | lowlands_center         | 检测凹地所有灰度值的中心               | 493  |
| 8    | plateaus                | 检测所有平稳状态灰度值                 | 494  |
| 9    | plateaus_center         | 检测所有平稳状态灰度值的中心           | 494  |
| 10   | pouring                 | 根据大于“pouring_water”分割图像        | 495  |
| 11   | saddle_points_sub_pix   | 一幅图像中底部点的子像素精确度检测     | 495  |
| 12   | watersheds              | 从一幅图像中提取分界线和“盆地”         | 496  |
| 13   | watersheds_threshold    | 利用阀值从一幅图像中提取“分水岭盆地”   | 496  |

## Chapter 22: System（系统）

### 22.1 Compute Devices   计算手段

| 序号 | 函数名                          | 函数说明及注释                     | 页码 |
| ---- | ------------------------------- | ---------------------------------- | ---- |
| 1    | activate_compute_device         | 激活指定计算设备（工业相机）       | 501  |
| 2    | deactivate_all_compute_devices  | 解除所有计算设备（工业相机）       | 501  |
| 3    | deactivate_compute_device       | 解除指定计算设备（工业相机）       | 501  |
| 4    | get_compute_device_info         | 获取指定计算设备的信息（工业相机） | 501  |
| 5    | get_compute_device_param        | 获取指定计算设备（工业相机）的参数 | 501  |
| 6    | init_compute_device             | 初始化指定计算设备（工业相机）     | 501  |
| 7    | open_compute_device             | 打开一个计算设备（工业相机）       | 502  |
| 8    | query_available_compute_devices | 获取可用的计算设备（工业相机）     | 502  |
| 9    | release_all_compute_devices     | 关闭所有的计算设备（工业相机）     | 502  |
| 10   | release_compute_device          | 关闭指定的计算设备（工业相机）     | 502  |
| 11   | set_compute_device_param        | 设置指定的计算设备（工业相机）参数 | 502  |

### 22.2 Database 数据库

| 序号 | 函数名         | 函数说明及注释             | 页码 |
| ---- | -------------- | -------------------------- | ---- |
| 1    | count_relation | 在HALCON数据库中实体的数目 | 502  |
| 2    | get_modules    | 查询已使用模块和模块关键码 | 502  |
| 3    | reset_obj_db   | HALCON系统的初始化         | 503  |

### 22.3 Error-Handing 错误处理

| 序号 | 函数名         | 函数说明及注释                 | 页码 |
| ---- | -------------- | ------------------------------ | ---- |
| 1    | get_check      | HALCON控制模式下被激活的列表   | 503  |
| 2    | get_error_text | 查询HALCON错误测试后错误数目   | 503  |
| 3    | get_spy        | HALCON调试工具当前配置         | 503  |
| 4    | query_spy      | 查询HALCON调试工具激活的设置   | 503  |
| 5    | set_check      | 设置被激活和钝化HALCON控制模式 | 503  |
| 6    | set_spy        | 设置HALCON控制模式的状态       | 503  |

### 22.4 Information  数据相关信息

| 序号 | 函数名              | 函数说明及注释                             | 页码 |
| ---- | ------------------- | ------------------------------------------ | ---- |
| 1    | get_chapter_info    | 获取程序有关章节的信息                     | 504  |
| 2    | get_keywords        | 获取指定给程序的关键字                     | 504  |
| 3    | get_operator_info   | 获取关于HALCON程序的信息                   | 504  |
| 4    | get_operator_name   | 获取由给定字符串作为它们的名字的程序       | 504  |
| 5    | get_param_info      | 获取关于程序参数的信息                     | 504  |
| 6    | get_param_names     | 获取一个HALCON程序参数的名字               | 505  |
| 7    | get_param_num       | 获取一个HALCON程序不同参数类的数目         | 505  |
| 8    | get_param_types     | 获取一个HALCON程序控制参数的缺省数据类型   | 505  |
| 9    | query_operator_info | 联合操作get_operator_info查询空挡相关信息  | 505  |
| 10   | query_param_info    | 查询关于操作get_param_info的空挡的在线信息 | 505  |
| 11   | search_operator     | 在程序进程中寻找一个关键字                 | 505  |

### 22.5 Multithreading	多线程

| 序号 | 函数名               | 函数说明及注释                                 | 页码 |
| ---- | -------------------- | ---------------------------------------------- | ---- |
| 1    | broadcast_condition  | 同步信号状态，复位所有正在等候的线程           | 506  |
| 2    | clear_all_barriers   | 清除所有的排斥对象                             | 506  |
| 3    | clear_all_conditions | 清除所有信号对象                               | 506  |
| 4    | clear_all_events     | 清除所有的事件对象                             | 506  |
| 5    | clear_all_mutexed    | 清除所有的互斥对象                             | 506  |
| 6    | clear_barrier        | 清除指定的排斥对象                             | 506  |
| 7    | clear_condition      | 清除指定信号对象                               | 506  |
| 8    | clear_event          | 清除指定的事件对象                             | 507  |
| 9    | clear_mutex          | 清除指定的互斥对象                             | 507  |
| 10   | create_barrier       | 创建一个排斥对象                               | 507  |
| 11   | create_condition     | 创建一个信号对象                               | 507  |
| 12   | create_event         | 创建一个事件对象                               | 507  |
| 13   | create_mutex         | 创建一个互斥对象                               | 507  |
| 14   | get_threading_attrib | 提取线程的属性                                 | 507  |
| 15   | lock_mutex           | 锁一个互斥对象                                 | 507  |
| 16   | signal_condition     | 信号对象的状态                                 | 507  |
| 17   | signal_event         | 开启事件对象                                   | 508  |
| 18   | timed_wait_condition | 等到同步信号跳转                               | 508  |
| 19   | try_lock_mutex       | 试图锁上一个互斥对象                           | 508  |
| 20   | try_wait_event       | 试图对一个事件进行上锁，一旦上锁，只有它能解锁 | 508  |
| 21   | unlock_mutex         | 解锁一个互斥对象                               | 508  |
| 22   | wait_barrier         | 等待释放一个排斥对象                           | 508  |
| 23   | wait_condition       | 等待一个信号对象                               | 508  |
| 24   | wait_event           | 等待指定事件的发生                             | 508  |

### 22.6 Operating-System	操作系统

| 序号 | 函数名        | 函数说明及注释 | 页码 |
| ---- | ------------- | -------------- | ---- |
| 1    | count_senonds | 衡量时间       | 509  |
| 2    | system_call   | 执行系统请求   | 509  |
| 3    | wait_senonds  | 延迟操作的执行 | 509  |

### 22.7 Parallelization	自动操作并行化（多核）

### 22.8 Parameters 参数

| 序号 | 函数名     | 函数说明及注释                       | 页码 |
| ---- | ---------- | ------------------------------------ | ---- |
| 1    | get_system | 根据HALCON系统参数获取关于当前的信息 | 509  |
| 2    | set_system | HALCON系统参数的设置                 | 509  |

### 22.9 Seial	串行操作

| 序号 | 函数名            | 函数说明及注释             | 页码 |
| ---- | ----------------- | -------------------------- | ---- |
| 1    | clear_serial      | 清除一个串行设备的缓冲内存 | 510  |
| 2    | close_all_serials | 关闭所有的串行设备         | 510  |
| 3    | close_serial      | 关闭一个串行设备           | 510  |
| 4    | get_serial_param  | 获取一个串行设备的参数     | 510  |
| 5    | open_serial       | 打开一个串行设备           | 510  |
| 6    | read_serial       | 读取一个串行设备           | 511  |
| 7    | set_serial_param  | 设置一个串行设备的参数     | 511  |
| 8    | write_serial      | 写入一个串行设备           | 511  |

### 22.10 Sockets	套接字（网络）

| 序号 | 函数名                    | 函数说明及注释                               | 页码 |
| ---- | ------------------------- | -------------------------------------------- | ---- |
| 1    | close_socket              | 关闭一个网络                                 | 512  |
| 2    | get_next_socket_data_type | 决定下一个网络数据的HALCON数据类型           | 512  |
| 3    | get_socket_descriptor     | 获取一个网络的描述符                         | 513  |
| 4    | get_socket_param          | 获取一个网络的参数                           | 513  |
| 5    | open_socket_accept        | 打开一个接受连接请求的网络                   | 513  |
| 6    | open_socket_connect       | 打开一个已存在的网络                         | 513  |
| 7    | receive_data              | 接收外部设备或一般信息通信工具发送过来的数据 | 513  |
| 8    | receive_image             | 通过网络接收一副图像                         | 513  |
| 9    | receive_region            | 通过网络接收区域                             | 513  |
| 10   | receive_tuple             | 通过网络接收一个元祖                         | 514  |
| 11   | receive_xld               | 通过网络接收一个XLD对象                      | 514  |
| 12   | send_data                 | 发送任意数据到外部设备或一般的信息通信工具   | 514  |
| 13   | send_image                | 通过网络发送一副图像                         | 514  |
| 14   | send_region               | 通过网络发送区域                             | 514  |
| 15   | send_tuple                | 通过网络发送一个元祖                         | 514  |
| 16   | send_xld                  | 通过网络发送一个XLD对象                      | 515  |
| 17   | set_socket_timeout        | 设置一个网络连接的超时                       | 515  |
| 18   | socket_accept_connect     | 接受一个监听网络的连接请求                   | 515  |

## Chapter 23 : Tools(工具)

### 23.1 	Background-Estimator	评估背景

| 序号 | 函数名             | 函数说明及注释                     | 页码 |
| ---- | ------------------ | ---------------------------------- | ---- |
| 1    | close_all_bg_esti  | 清除所有的背景评估数据集           | 519  |
| 2    | close_bg_esti      | 清除背景估测数据集                 | 519  |
| 3    | create_bg_esti     | 创建一个背景评估数据集并进行初始化 | 519  |
| 4    | get_bg_esti_params | 提取一个数据集的参数               | 520  |
| 5    | give_bg_esti       | 提取一个背景评估图像               | 520  |
| 6    | run_bg_esti        | 评估背景并返回前景区域             | 520  |
| 7    | set_bg_esti_params | 设置背景评估数据集的参数           | 520  |
| 8    | update_bg_esti     | 改变估测背景图像                   | 520  |

### 23.2	Function	函数

| 序号 | 函数名                  | 函数说明及注释                   | 页码 |
| ---- | ----------------------- | -------------------------------- | ---- |
| 1    | abs_funct_1d            | Y值的绝对值                      | 522  |
| 2    | compose_funct_1d        | 组合两个函数操作                 | 522  |
| 3    | create_funct_1d_array   | 从Y值的序列中创建一个函数        | 522  |
| 4    | create_funct_1d_pairs   | 从（X、Y）集合中创建一个函数     | 522  |
| 5    | derivate_funct_1d       | 计算一个函数的派生物             | 522  |
| 6    | distance_funct_1d       | 计算两个函数的间隔               | 523  |
| 7    | funct_1d_to_pairs       | 查询一个函数的（X、Y）值         | 523  |
| 8    | get_pair_funct_1d       | 根据控制点的索引查询一个函数值   | 523  |
| 9    | get_y_value_funct_1d    | 返回任意位置函数的值             | 524  |
| 10   | integrate_funct_1d      | 计算一个函数的正区域和负区域     | 524  |
| 11   | invert_funct_1d         | 计算一个函数的反转               | 524  |
| 12   | local_min_max_funct_1d  | 计算一个函数的局域最小和最大值点 | 524  |
| 13   | match_funct_1d_trans    | 计算两个函数传递参数             | 525  |
| 14   | negate_funct_1d         | 对Y值取非（反）                  | 525  |
| 15   | num_points_funct_1d     | 函数控制点的数目                 | 525  |
| 16   | read_funct_1d           | 从文件中读取一个函数             | 526  |
| 17   | sample_funct_1d         | 再间隔区等距取样                 | 526  |
| 18   | scale_y_funct_1d        | 将Y值相乘和相加                  | 526  |
| 19   | smooth_funct_1d_gauss   | 采用高斯函数平滑一个等距一维函数 | 526  |
| 20   | smooth_funct_1d_mean    | 采用平均函数平滑一个等距一维函数 | 527  |
| 21   | transform_funct_1d      | 根据给定传递参数变换一个函数     | 527  |
| 22   | write_funct_1d          | 将一个函数写入一个文件           | 527  |
| 23   | x_range_funct_1d        | 函数的最小和最大X值              | 527  |
| 24   | y_range_funct_1d        | 函数的最小和最大Y值              | 527  |
| 25   | zero_crossings_funct_1d | 计算一个函数的的零点             | 528  |

### 23.3	Geometry	几何学

| 序号 | 函数名              | 函数说明及注释                                   | 页码 |
| ---- | ------------------- | ------------------------------------------------ | ---- |
| 1    | angle_ll            | 计算两条线的夹角                                 | 528  |
| 2    | angle_lx            | 计算一条线与垂直轴之间的角度                     | 529  |
| 3    | distance_cc         | 计算两个轮廓间的距离                             | 529  |
| 4    | distance_cc_min     | 计算两个轮廓间的最小距离                         | 530  |
| 5    | distance_lc         | 计算一条线和一个轮廓间的距离                     | 530  |
| 6    | distance_lr         | 计算一条线和一个区域间的距离                     | 530  |
| 7    | distance_pc         | 计算一个点和一个轮廓间的距离                     | 531  |
| 8    | distance_pl         | 计算一个点和一条线间的直交距离                   | 532  |
| 9    | distance_pp         | 计算两个点之间的直线距离                         | 533  |
| 10   | distance_pr         | 计算一个点和一个区域间的距离                     | 534  |
| 11   | distance_ps         | 计算一个点和一条线段间的距离                     | 534  |
| 12   | distance_rr_min     | 计算两个相邻区域之间的最小距离，并给出对应的坐标 | 535  |
| 13   | distance_rr_min_dil | 计算两个区域间的最小距离                         | 536  |
| 14   | distance_sc         | 计算一条线段和一个轮廓间的距离                   | 536  |
| 15   | distance_sl         | 计算一条线段和一条线间的距离                     | 537  |
| 16   | distance_sr         | 计算一条线段和一个区域间的距离                   | 537  |
| 17   | distance_ss         | 计算两条线段间的距离                             | 537  |
| 18   | get_points_ellipse  | 计算椭圆上特定角度的一个点                       | 538  |
| 19   | intersection_ll     | 计算两条线的交集点（相交点）                     | 539  |
| 20   | projection_pl       | 计算一条线上的一个点的投影                       | 540  |
| 21   | sort_pairs          | 成对分类                                         | 540  |

### 23.4	Grid-Rectification	网络

| 序号 | 函数名                       | 函数说明及注释                                       | 页码 |
| ---- | ---------------------------- | ---------------------------------------------------- | ---- |
| 1    | connect_grid_points          | 简历矫正网络的各格点间的连接                         | 541  |
| 2    | create_rectification_grid    | 建立一个附文件，描述矫正网络                         | 541  |
| 3    | find_rectification_grid      | 分割图像中网络区域                                   | 541  |
| 4    | gen_arbitrary_distortion_map | 产生一个投射图，其描述随意扭曲图像与正确图像间的映射 | 541  |
| 5    | gen_grid_rectification_map   | 计算扭曲图像与基于规律的网格的正确的图像的映射       | 542  |

### 23.5	Hough	（hough变换）

| 序号 | 函数名                | 函数说明及注释                                 | 页码 |
| ---- | --------------------- | ---------------------------------------------- | ---- |
| 1    | hough_circle_trans    | 返回指定半径的圆周的Hough变换                  | 543  |
| 2    | hough_circles         | 特定半径的圆周的中心                           | 543  |
| 3    | hough_line_trans      | 对区域中的线进行Hough变换                      | 544  |
| 4    | hough_line_trans_dir  | 利用局部方向梯度对线进行Hough变换              | 544  |
| 5    | hough_lines           | 借助Hough变化查询图像中的线，并将其返回到HNF中 | 544  |
| 6    | hough_lines_dir       | 采用局部方向梯度的Hough变换查询图像中的线      | 544  |
| 7    | select_matching_lines | 选取HNF中线的集合中匹配区域最好的线            | 545  |

### 23.6	Kalman-Filter	卡尔曼滤波器

| 序号 | 函数名        | 函数说明及注释                     | 页码 |
| ---- | ------------- | ---------------------------------- | ---- |
| 1    | filter_kalman | 借助卡尔曼滤波器估测系统的当前状态 | 545  |
| 2    | read_kalman   | 读取一个卡尔曼滤波器的说明文件     | 545  |
| 3    | update_kalman | 读取一个卡尔曼滤波器的更新文件     | 545  |

### 23.7	Lines	线性

| 序号 | 函数名               | 函数说明及注释               | 页码 |
| ---- | -------------------- | ---------------------------- | ---- |
| 1    | approx_chain         | 通过弧和线近似一个轮廓       | 546  |
| 2    | approx_chain_simple  | 通过弧和线近似一个轮廓       | 546  |
| 3    | line_orientation     | 计算线的方位                 | 547  |
| 4    | line_position        | 计算一条线的重心、长度和方位 | 547  |
| 5    | partition_lines      | 通过特征选择分割线段         | 548  |
| 6    | select_lines         | 通过特征选择线               | 548  |
| 7    | select_lines_longest | 选择最长输入线               | 549  |

### 23.8	Mosaicking	（马赛克图像）

| 序号 | 函数名                          | 函数说明及注释                                           | 页码 |
| ---- | ------------------------------- | -------------------------------------------------------- | ---- |
| 1    | adjust_mosaic_images            | 全景图像的自动颜色更改                                   | 549  |
| 2    | bundle_adjust_mosaic            | 对一幅图像的嵌合体采取一系列校正                         | 549  |
| 3    | gen_bundle_adjusted_mosaic      | 把多重图像合成一个马赛克图像                             | 550  |
| 4    | gen_cube_map_mosaic             | 创建立方体马赛克图像（含6方位图像）                      | 550  |
| 5    | gen_projective_mosaic           | 把多重图像合成一个马赛克图像                             | 550  |
| 6    | gen_spherical_mosaic            | 创建一个球形马赛克图像                                   | 551  |
| 7    | proj_match_points_ransack       | 找两图图像中点与点之间的映射计算一个投影变换矩阵         | 551  |
| 8    | proj_match_points_ransac_guided | 找两个图像中点与点和一个近似变换矩阵来计算投射变形点阵式 | 552  |

## Chapter 24 : Transformations	(转换)

### 24.1	2D Transformations	2D转换

| 序号 | 函数名                       | 函数说明及注释                                   | 页码 |
| ---- | ---------------------------- | ------------------------------------------------ | ---- |
| 1    | affine_trans_pixel           | 对像素坐标轴进行任意的放射二维变换               | 555  |
| 2    | affine_trans_point_2d        | 对点进行任意的最简二维变换                       | 555  |
| 3    | hom_mat2d_compose            | 将两种相同类型二维变换矩阵相乘                   | 556  |
| 4    | hom_mat2d_determinant        | 计算一个同质的二维变换矩阵的行列式               | 556  |
| 5    | hom_mat2d_identity           | 构建二维变换同样的同质变换矩阵                   | 556  |
| 6    | hom_mat2d_invert             | 插入一个同质二维变换矩阵                         | 556  |
| 7    | hom_mat2d_rotate             | 为一个同质二维变换矩阵添加一个旋转               | 556  |
| 8    | hom_mat2d_rotate_local       | 为一个同质二维变换矩阵添加一个旋转（以指定位置） | 556  |
| 9    | hom_mat2d_scale              | 为一个同质二维变换矩阵添加一个缩放               | 556  |
| 10   | hom_mat2d_scale_local        | 为一个同质二维变换矩阵添加一个缩放（以指定位置） | 556  |
| 11   | hom_mat2d_slant              | 为一个同质二维变换矩阵添加一个拉伸               | 557  |
| 12   | hom_mat2d_slant_local        | 为一个同质二维变换矩阵添加一个拉伸（以指定位置） | 557  |
| 13   | hom_mat2d_to_affine_par      | 计算一个来自一个同质二维变换矩阵的仿射变换参数   | 557  |
| 14   | hom_mat2d_translate          | 为一个同质二维变换矩阵添加一个平移               | 557  |
| 15   | hom_mat2d_translate_local    | 为一个同质二维变换矩阵添加一个平移（以指定位置） | 557  |
| 16   | hom_mat2d_transpose          | 将一个同质二维变换矩阵（行列）转置               | 558  |
| 17   | hom_mat3d_project            | 给一个二维投影变换矩阵投影一个仿射三维变换矩阵   | 558  |
| 18   | hom_vector_to_proj_hom_mat2d | 根据给定点的映射计算一个同质变换矩阵             | 558  |
| 19   | projective_trans_pixel       | 利用一个同质投影变换矩阵表示像素坐标轴           | 558  |
| 20   | projective_trans_point_2d    | 利用一个投影变换矩阵计算一个同质二维点           | 558  |
| 21   | vertor_angle_to_rigid        | 通过点和角度方面来计算一个仿射变换矩阵           | 558  |
| 22   | vector_field_to_hom_mat2d    | 根据唯一矢量字段获取一个近似的二维变换矩阵       | 559  |
| 23   | vertor_to_hom_mat2d          | 根据点与点间的映射获取一个近似的二维变换矩阵     | 559  |
| 24   | vertor_to_proj_hom_mat2d     | 根据给定点的映射计算一个映射变换矩阵             | 559  |
| 25   | vector_to_rigid              | 根据点的映射获取一个近似严格的放射变换           | 559  |
| 26   | vector_to_similarity         | 根据点的映射获取一个近似的相似变换               | 560  |

### 24.2	3D-Transformations	3D转换

| 序号 | 函数名                    | 函数说明及注释                                         | 页码 |
| ---- | ------------------------- | ------------------------------------------------------ | ---- |
| 1    | affine_trrans_point_3d    | 对点运用一个随即仿射三维变换                           | 560  |
| 2    | hom_mat3d_compose         | 将两个同质三维变换矩阵相乘                             | 560  |
| 3    | hom_mat3d_identity        | 创建一个三维变换同样的同质变换矩阵                     | 561  |
| 4    | hom_mat3d_invert          | 插入一个同质三维变换矩阵                               | 561  |
| 5    | hom_mat3d_rotate          | 为一个同质三维变换矩阵添加一个旋转，以定位点为参考坐标 | 561  |
| 6    | hom_mat3d_rotate_local    | 为一个同质三维变换矩阵添加一个旋转，以原点为参考坐标   | 561  |
| 7    | hom_mat3d_scale           | 为一个同质三维变换矩阵添加一个缩放，以定位点为参考坐标 | 561  |
| 8    | hom_mat3d_scale_local     | 为一个同质三维变换矩阵添加一个缩放，以原点为参考坐标   | 562  |
| 9    | hom_mat3d_to_pose         | 将一个同质变换矩阵转换为一个三维模式                   | 562  |
| 10   | hom_mat3d_translate       | 为一个同质三维变换矩阵添加一个旋转                     | 562  |
| 11   | hom_mat3d_translate_local | 为一个同质三维变换矩阵添加一个旋转                     | 562  |
| 12   | pose_to_hom_mat3d         | 将一个三维模式转换为一个同质变换矩阵                   | 562  |

### 24.3	Misc	混合

| 序号 | 函数名                         | 函数说明及注释                       | 页码 |
| ---- | ------------------------------ | ------------------------------------ | ---- |
| 1    | convert_point_3d_cart_to_spher | 把直角坐标系中的一个3D点转变为极坐标 | 563  |
| 2    | convert_point_3d_spher_to_cart | 把极坐标中的一个3D点转变为直角坐标   | 563  |
| 3    | get_line_of_sight              | 计算相应于图像中一个点的视线         | 563  |

### 24.4	Poses	伪装

| 序号 | 函数名                 | 函数说明及注释                               | 页码 |
| ---- | ---------------------- | -------------------------------------------- | ---- |
| 1    | convert_pose_type      | 改变一个三维系的方位                         | 564  |
| 2    | create_pose            | 创建一个三维坐标系                           | 564  |
| 3    | get_circle_pose        | 从一个圆周相应的二维投射中决定它的三维模式   | 564  |
| 4    | get_pose_type          | 获取一个三维系的方位                         | 564  |
| 5    | get_rectangle_pose     | 从一个矩形相应的二维投射中决定它的三维模式   | 564  |
| 6    | proj_hom_mat2d_to_pose | 把一个世界坐标转换为图像坐标                 | 565  |
| 7    | quat_to_pose           | 把一个四元数转换为三维坐标系                 | 565  |
| 8    | read_pose              | 从一个文本文件中读取一个三维坐标系           | 566  |
| 9    | set_origin_pose        | 设置一个三维坐标系的原点                     | 566  |
| 10   | vector_to_pose         | 计算世界坐标（绝对坐标）和图像坐标之间的转换 | 566  |
| 11   | write_pose             | 将一个三维坐标系写入一个文本文件             | 567  |

### 24.5	Quaternions	四元法

| 序号 | 函数名               | 函数说明及注释                   | 页码 |
| ---- | -------------------- | -------------------------------- | ---- |
| 1    | axis_angle_to_quat   | 创建一个四元数                   | 566  |
| 2    | quat_compose         | 两四元数相乘                     | 566  |
| 3    | quat_conjugate       | 产生一个四元数的结合             | 566  |
| 4    | quat_interpolate     | 对两个四元组进行篡改             | 566  |
| 5    | quat_normalize       | 对一个四元数进行常态化（归一化） | 567  |
| 6    | quat_rotate_point_3d | 对四元数进行一次旋转操作         | 567  |
| 7    | quat_to_hom_mat3d    | 把四元数转换成旋转矩阵式         | 567  |

## Chapter 25 : Tuple	(元组)

### 25.1	Arithmetic	运算

| 序号 | 函数名      | 函数说明及注释                     | 页码 |
| ---- | ----------- | ---------------------------------- | ---- |
| 1    | tuple_abs   | 计算一个元组的绝对值               | 571  |
| 2    | tuple_acos  | 计算一个元组的反余弦               | 571  |
| 3    | tuple_add   | 两个元组相加                       | 572  |
| 4    | tuple_asin  | 计算一个元组的反正弦               | 572  |
| 5    | tuple_atan  | 计算一个元组的反正切               | 572  |
| 6    | tuple_atan2 | 计算一个元组四个象限的反正切       | 572  |
| 7    | tuple_ceil  | 计算一个元组的上限函数             | 572  |
| 8    | tuple_cos   | 计算一个元组的余弦                 | 572  |
| 9    | tuple_cosh  | 计算一个元组的双曲余弦             | 572  |
| 10   | tuple_cumul | 计算一个元组的累计加               | 572  |
| 11   | tuple_deg   | 将一个元组从弧度转换为角度         | 572  |
| 12   | tuple_div   | 将两个元组相除                     | 573  |
| 13   | tuple_exp   | 元组的指数运算                     | 573  |
| 14   | tuple_fabs_ | 计算一个元组（例如浮点数）的绝对值 | 573  |
| 15   | tuple_floor | 计算一个元组的“地板函数”           | 573  |
| 16   | tuple_fmod  | 计算两个元组浮点数相除的余数       | 573  |
| 17   | tuple_ldexp | 计算两个元组的返回长双精度指数函数 | 573  |
| 18   | tuple_log   | 计算一个元组的自然对数             | 573  |
| 19   | tuple_log10 | 计算一个元组底为10的对数           | 573  |
| 20   | tuple_max2  | 计算两个元组的元素宽度的最大值     | 574  |
| 21   | tuple_min2  | 计算两个元组的元素宽度的最小值     | 574  |
| 22   | tuple_mod   | 计算两个元组整形数相除的余数       | 574  |
| 23   | tuple_mult  | 两个元组相乘                       | 574  |
| 24   | tuple_neg   | 将一个元组取反                     | 574  |
| 25   | tuple_pow   | 计算两个元组的冥函数               | 574  |
| 26   | tuple_rad   | 将一个元组从角度转换为弧度         | 574  |
| 27   | tuple_sgn   | 计算一个元组的正负                 | 574  |
| 28   | tuple_sin   | 计算一个元组的正弦                 | 575  |
| 29   | tuple_sinh  | 计算一个元组的双曲正弦             | 575  |
| 30   | tuple_sqrt  | 计算一个元组的平方根（二次方根）   | 575  |
| 31   | tuple_sub   | 两个元组相减                       | 575  |
| 32   | tuple_tan   | 计算一个元组的正切                 | 575  |
| 33   | tuple_tanh  | 计算一个元组的双曲正切             | 575  |

### 25.2	Bit-Operations	位操作

| 序号 | 函数名     | 函数说明及注释         | 页码 |
| ---- | ---------- | ---------------------- | ---- |
| 1    | tuple_band | 计算两个元组的运算     | 575  |
| 2    | tuple_bnot | 元组逻辑非运算         | 576  |
| 3    | tuple_bor  | 计算两个元组的运算     | 576  |
| 4    | tuple_bxor | 计算两个元组的异或运算 | 576  |
| 5    | tuple_lsh  | 元组逐位左移           | 576  |
| 6    | tuple_rsh  | 元组逐位右移           | 576  |

### 25.3	Comparison	对比

| 序号 | 函数名              | 函数说明及注释                 | 页码 |
| ---- | ------------------- | ------------------------------ | ---- |
| 1    | tuple_equal         | 测试两个元组是否相同           | 577  |
| 2    | tuple_greater       | 测试一个元组是否大于另一个元组 | 577  |
| 3    | tuple_greater_equal | 测试一个元组是否大于等于另一个 | 577  |
| 4    | tuple_less          | 测试一个元组是否小于另一个元组 | 577  |
| 5    | tuple_less_equal    | 测试一个元组是否小于等于另一个 | 577  |
| 6    | tuple_less_equal    | 测试两个元组是否不相等         | 577  |

### 25.4	Conversion	变换/转化

| 序号 | 函数名          | 函数说明及注释                            | 页码 |
| ---- | --------------- | ----------------------------------------- | ---- |
| 1    | tuple_chr       | 根据ASCII码将整型元组转换为字符元组       | 578  |
| 2    | tuple_chrt      | 根据ASCII码将整型元组转换为字符串         | 578  |
| 3    | tuple_int       | 将一个元组转换为一个整型元组              | 578  |
| 4    | tuple_is_number | 检测一个字符串元组是否表示数字            | 578  |
| 5    | tuple_number    | 将一个字符串元组转换为一个数字元组        | 578  |
| 6    | tuple_ord       | 将一个字符串的元组转换为对应的ASCII码整数 | 578  |
| 7    | tuple_ords      | 将一个字符串的元组转换为它们ASCII码的元组 | 579  |
| 8    | tuple_real      | 将一个元组转换为一个浮点数的元组          | 579  |
| 9    | tuple_round     | 将一个元组转换为一个整型数的元组          | 579  |
| 10   | tuple_string    | 将一个元组转换为一个字符串元组            | 579  |

### 25.5	Creation	创建

| 序号 | 函数名             | 函数说明及注释                            | 页码 |
| ---- | ------------------ | ----------------------------------------- | ---- |
| 1    | tuple_concat       | 合并两个元组为一个新的                    | 580  |
| 2    | tuple_gen_const    | 创建指定长度并初始化该元组                | 580  |
| 3    | tuple_rand         | 创建指定长度并初始化0-1之间的任意值的元组 | 580  |
| 4    | tuple_gen_sequence | 按指定步长初始化一个元组                  | 580  |

### 25.6	Element-Order	排序

| 序号 | 函数名           | 函数说明及注释                   | 页码 |
| ---- | ---------------- | -------------------------------- | ---- |
| 1    | tuple_inverse    | 将一个元组反置排序（反转）       | 580  |
| 2    | tuple_sort       | 按照升序排序                     | 581  |
| 3    | tuple_sort_index | 将元组的元素排序并返回元组的索引 | 581  |

### 25.7	Features	特征

| 序号 | 函数名            | 函数说明及注释           | 页码 |
| ---- | ----------------- | ------------------------ | ---- |
| 1    | tuple_devistion   | 返回一个元组元素的标注差 | 581  |
| 2    | tuple_histo_range | 计算一个元组的正态分布图 | 581  |
| 3    | tuple_length      | 返回一个元组元素数目     | 582  |
| 4    | tuple_max         | 返回一个元组的最大元素   | 582  |
| 5    | tuple_mean        | 返回一定数量元组的平均值 | 582  |
| 6    | tuple_median      | 返回一个元组元素的中值   | 582  |
| 7    | tuple_min         | 返回一个元组的最小元素   | 582  |
| 8    | tuple_sum         | 返回一个元组所有元素的和 | 582  |

### 25.8	Logic-Operations	逻辑运算

| 序号 | 函数名    | 函数说明及注释     | 页码 |
| ---- | --------- | ------------------ | ---- |
| 1    | tuple_and | 两个元组的逻辑与   | 583  |
| 2    | tuple_not | 两个元组的逻辑非   | 583  |
| 3    | tuple_or  | 两个元组的逻辑或   | 583  |
| 4    | tuple_xor | 两个元组的逻辑异或 | 583  |

### 25.9	Selection	选择

| 序号 | 函数名               | 函数说明及注释                                 | 页码 |
| ---- | -------------------- | ---------------------------------------------- | ---- |
| 1    | tuple_find           | 找出第2元组对应元组在第1元组对应的位置（索引） | 584  |
| 2    | tuple_first_n        | 选取一个元组的前几个元素                       | 584  |
| 3    | tuple_last_n         | 选择从符号“n”开始到元组末尾的所有元素          | 584  |
| 4    | tuple_remove         | 从一个元组中移出元素                           | 584  |
| 5    | tuple_select         | 选择一个元组中单一元素                         | 585  |
| 6    | tuple_select_range   | 选择一个元组中的两索引间的连续元素             | 585  |
| 7    | tuple_select_rank    | 选择一个元组中序号为n的元素                    | 585  |
| 8    | tuple_str_bit_select | 选择一个元组中单一符号或位                     | 585  |
| 9    | tuple_uniq           | 相邻重叠的元组数只保留一个                     | 585  |

### 25.10	String-Operators	字符串操作

| 序号 | 函数名               | 函数说明及注释                              | 页码 |
| ---- | -------------------- | ------------------------------------------- | ---- |
| 1    | tuple_environment    | 读取一个或多个环境变量                      | 586  |
| 2    | tuple_regexp_match   | 从字符串中提取配对的字符                    | 586  |
| 3    | tuple_regexp_replace | 用有规律的公式替代一个子链                  | 587  |
| 4    | tuple_regexp_select  | 选择符合公式的元组元素                      | 587  |
| 5    | tuple_regexp_test    | 测试一个字符串是否满足一个规则公式的要求    | 588  |
| 6    | tuple_split          | 在预定义的独立字符间将字符串分离为子链      | 588  |
| 7    | tuple_str_first_n    | 分割从第一个字符直到字符串元组外的位置“n”处 | 588  |
| 8    | tuple_str_last_n     | 从字符串元组外位置“n”处开始分割所有的字符   | 589  |
| 9    | tuple_strchr         | 向前搜索一个位于字符串元组内的字符          | 589  |
| 10   | tuple_strlen         | 字符串元组中每个字符串的长度                | 589  |
| 11   | tuple_strrchr        | 向后搜索一个位于字符串元组内的字符          | 589  |
| 12   | tuple_strrstr        | 向后搜索一个位于字符串元组内的字符串        | 590  |
| 13   | tuple_strstr         | 向前搜索一个位于字符串元组内的字符串        | 590  |

## Chapter 26 : XLD	轮廓处理

### 26.1	Access	数据

| 序号 | 函数名            | 函数说明及注释        | 页码 |
| ---- | ----------------- | --------------------- | ---- |
| 1    | get_contour_xld   | 返回XLD轮廓的坐标     | 593  |
| 2    | get_lines_xld     | 返回一个XLD多边形数据 | 593  |
| 3    | get_parallers_xld | 返回一个XLD并行数据   | 594  |
| 4    | get_polygon_xld   | 返回一个XLD多边形数据 | 595  |

### 26.2	Creation	创建

| 序号 | 函数名                          | 函数说明及注释                                            | 页码 |
| ---- | ------------------------------- | --------------------------------------------------------- | ---- |
| 1    | gen_circle_contour_xld          | 创建一个圆或圆弧轮廓                                      | 596  |
| 2    | gen_contor_nurbs_xld            | 将一个NURBS曲线转换为一个XLD轮廓                          | 596  |
| 3    | gen_contour_polygon_rounded_xld | 根据一个多边形（以元组形式给出）的圆形角点创建一个XLD轮廓 | 597  |
| 4    | gen_contour_polygon_xld         | 根据一个多边形（以元组形式给出）创建一个XLD轮廓           | 597  |
| 5    | gen_contour_region_xld          | 根据区域创建XLD轮廓                                       | 598  |
| 6    | gen_contours_skeleton_xld       | 将骨骼框架转换为XLD轮廓                                   | 598  |
| 7    | gen_cross_contour_xld           | 根据每个输入点交叉的形状创建一个XLD轮廓                   | 599  |
| 8    | gen_ellipse_contour_xld         | 根据相应的椭圆弧创建一个XLD轮廓                           | 599  |
| 9    | gen_nurbs_interp                | 创建一个NURBS曲线轮廓                                     | 600  |
| 10   | gen_parallels_xld               | 提取并行XLD多边形                                         | 600  |
| 11   | gen_polygons_xld                | 根据多边形近似创建XLD轮廓                                 | 601  |
| 12   | gen_rectangle2_contour_xld      | 创建一个矩形XLD轮廓                                       | 601  |
| 13   | mod_parallels_xld               | 提取一个包括同质区域的并行XLD多边形，清除多重并行线       | 602  |
| 14   | gen_arrow_contour_xld           | 创建箭头形状的轮廓                                        | 602  |

### 26.3	Features	特征

| 序号 | 函数名                             | 函数说明及注释                                               | 页码 |
| ---- | ---------------------------------- | ------------------------------------------------------------ | ---- |
| 1    | area_center_points_xld             | 被看做点云的轮廓和多边形的面积和重心                         | 604  |
| 2    | area_center_xld                    | 轮廓和多边形的面积和重心                                     | 604  |
| 3    | circularity_xld                    | 影响轮廓或多边形圆度（与圆相近的程度）的形状系数             | 604  |
| 4    | compactness_xld                    | 影响轮廓或多边形致密性的形状系数                             | 604  |
| 5    | contour_point_num_xld              | 返回一个XLD轮廓上点的数目                                    | 604  |
| 6    | convexity_xld                      | 影响轮廓或多边形凹凸性的形状系数                             | 604  |
| 7    | diameter_xld                       | 两个轮廓或多边形上的点与指定坐标的直线距离                   | 605  |
| 8    | dist_ellipse_contour_points_xld    | 计算所有轮廓边沿上所有点到一个椭圆边沿最近的距离             | 605  |
| 9    | dist_ellipse_cnotour_xld           | 轮廓到一个椭圆的最近距离的最小、最大、平均、标准差           | 605  |
| 10   | dist_rectangle2_contour_points_xld | 计算所有轮廓边沿上所有点到一个矩形边沿最近的距离             | 605  |
| 11   | eccentricity_points_xld            | 提取一个等高线轮廓或多边形的对称性                           | 605  |
| 12   | eccentricity_xld                   | 提取一个等高线轮廓或多边形的对称性和肥胖型                   | 606  |
| 13   | elliptic_axis_points_xld           | 提取类似椭圆的轮廓线或多边形的等价椭圆参数                   | 606  |
| 14   | elliptic_axis_xld                  | 提取类似椭圆的轮廓线或多边形的等价椭圆参数                   | 606  |
| 15   | fit_circle_contour_xld             | 根据一个类似圆（或圆弧）的等高线轮廓来提取一个标准圆         | 606  |
| 16   | fit_ellipse_contour_xld            | 根据一个类似于椭圆（或椭圆弧）的等高线轮廓来提取一个标注椭圆 | 607  |
| 17   | fit_line_contour_xld               | 根据一个类似线的等高线轮廓来提取一个标准差                   | 609  |
| 18   | fit_rectangle2_contour_xld         | 根据一个类似矩形的等高线轮廓来提取一个标准的矩形             | 610  |
| 19   | get_contour_angle_xld              | 为每个轮廓点计算一个XLD轮廓方向                              | 611  |
| 20   | get_contour_attrib_xld             | 返回一个XLD轮廓的点的特征值                                  | 611  |
| 21   | get_contour_global_attrib_xld      | 返回一个XLD轮廓的全局特征值                                  | 611  |
| 22   | get_regress_params_xld             | 返回XLD轮廓参数                                              | 612  |
| 23   | info_parallels_xld                 | 返回被XLD多边形包围的区域的平行质量及灰度值的信息            | 612  |
| 24   | length_xld                         | 轮廓或多边形的长度                                           | 613  |
| 25   | local_max_contours_xld             | 选择局域最大灰度值的XLD轮廓                                  | 613  |
| 26   | max_parallers_xld                  | 最大化的合并或延长并行轮廓                                   | 613  |
| 27   | moments_any_points_xld             | 被看做点云的轮廓或多边形的任意几何时刻                       | 614  |
| 28   | moments_any_xld                    | 轮廓或多边形的任意几何时刻                                   | 614  |
| 29   | moments_points_xld                 | 被看做点云的轮廓或多边形的几何时刻M20, M02, 和M11            | 614  |
| 30   | moments_xld                        | 轮廓或多边形的几何时刻M20, M02, 和M11                        | 615  |
| 31   | orientation_points_xld             | 被看做点云的轮廓或多边形的方向                               | 615  |
| 32   | orientation_xld                    | 轮廓或多边形的方向                                           | 615  |
| 33   | query_contour_arrribs_xld          | 返回一个XLD轮廓定义的属性的名字                              | 615  |
| 34   | query_contour_global_attribs_xld   | 返回一个XLD轮廓定义的全局属性的名字                          | 615  |
| 35   | select_contours_xld                | 根据一些特征选择XLD轮廓                                      | 615  |
| 36   | select_shape_xld                   | 根据形状特征选择轮廓或多边形                                 | 615  |
| 37   | select_xld_point                   | 选择包括给定点在内的所有的轮廓或多边形                       | 616  |
| 38   | smallest_circle_xld                | 轮廓或多边形的最小封闭圆                                     | 616  |
| 39   | smallest_rectangle1_xld            | 平行与轮廓或多边形的坐标轴的封闭矩形                         | 616  |
| 40   | smallest_rectangle2_xld            | 轮廓或多边形任意方向的最小封闭矩形                           | 617  |
| 41   | test_self_intersection_xld         | 测试轮廓或多边形自身相交性                                   | 617  |
| 42   | test_xld_point                     | 测试一个或多个轮廓或多边形是否寄附在给定点上                 | 618  |

### 26.4	Geometric-Transformations	几何变换

| 序号 | 函数名                       | 函数说明及注释                           | 页码 |
| ---- | ---------------------------- | ---------------------------------------- | ---- |
| 1    | affine_trans_contour_xld     | 对XLD轮廓进行一个任意二维仿射变换        | 618  |
| 2    | affine_trans_polygon_xld     | 对XLD多边形进行一个任意仿射变换          | 618  |
| 3    | gen_parallel_contour_xld     | 计算一个XLD轮廓的平行轮廓                | 619  |
| 4    | polar_trans_contour_xld      | 将一个环状弧中的轮廓转换为极坐标形式     | 619  |
| 5    | polar_trans_contour_xld_inv  | 将极坐标下的轮廓转换为笛卡尔坐标下的形式 | 619  |
| 6    | projective_trans_contour_xld | 对一个XLD轮廓进行射影变换                | 619  |

### 26.5	Sets	集合

| 序号 | 函数名                              | 函数说明及注释       | 页码 |
| ---- | ----------------------------------- | -------------------- | ---- |
| 1    | difference_closed_contours_xld      | 闭合轮廓的差异       | 620  |
| 2    | difference_closed_polygons_xld      | 闭合多边形的差异     | 620  |
| 3    | intersection_closed_contours_xld    | 闭合轮廓的交集       | 620  |
| 4    | intersection_closed_polygons_xld    | 闭合多边形的交集     | 621  |
| 5    | symm_difference_closed_contours_xld | 闭合轮廓的对称差异   | 621  |
| 6    | symm_difference_closed_polygons_xld | 闭合多边形的对称差异 | 622  |
| 7    | union2_closed_contours_xld          | 闭合轮廓的并集       | 622  |
| 8    | union2_closed_polygons_xld          | 闭合多边形的并集     | 622  |

### 26.6	Transformation	转换

| 序号 | 函数名                            | 函数说明及注释                       | 页码 |
| ---- | --------------------------------- | ------------------------------------ | ---- |
| 1    | add_noise_white_contour_xld       | 向XLD轮廓中加入噪声                  | 623  |
| 2    | clip_contours_xld                 | 修剪矩形内的等高线                   | 623  |
| 3    | clip_end_points_contours_xld      | 修剪等高线轮廓（按点分割或修剪长度） | 623  |
| 4    | close_contours_xld                | 封闭一个XLD轮廓                      | 624  |
| 5    | combine_roads_xld                 | 合并两个等级分辨率中的路（ road）    | 624  |
| 6    | crop_contours_xld                 | 切割一个XLD轮廓                      | 624  |
| 7    | merge_cont_line_scan_xld          | 合并连续线扫描图像中的XLD轮廓        | 624  |
| 8    | regress_contours_xld              | 计算一个XLD轮廓回归线的参数          | 625  |
| 9    | segment_contours_xld              | 将XLD轮廓分割为分割线和圆周或椭圆弧  | 625  |
| 10   | shape_trans_xld                   | 改变轮廓或多边形的形状               | 626  |
| 11   | smooth_contours_xld               | XLD轮廓的平滑                        | 626  |
| 12   | sort_contours_xld                 | 输入要排序的等高线                   | 626  |
| 13   | split_contours_xld                | 在主要点分割XLD轮廓                  | 626  |
| 14   | union_adjacent_contours_xld       | 合并终点连接在一起的轮廓             | 627  |
| 15   | union_cocircular_contours_xld     | 合并输入同一个圆周的轮廓             | 627  |
| 16   | union_collinear_contours_ext_xld  | 合并位于同一条圆上的圆弧轮廓         | 628  |
| 17   | union_collinear_contours_xld      | 合并位于同一条直线上的轮廓           | 628  |
| 18   | union_cotangential_contours_xld   | 合并具有切线关系的轮廓               | 629  |
| 19   | union_straight_contours_histo_xld | 合并到给定现有相似距离的相邻直线轮廓 | 630  |
| 20   | union_straight_contours_xld       | 合并具有相似方向的相邻直线轮廓       | 630  |
| 21   | track_wire                        | 电线路径查找                         | 631  |