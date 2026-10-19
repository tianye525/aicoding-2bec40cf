# 执行路线与恢复

助手先读根 AGENTS、manifest/services、当前进度和本轮材料，再按目标调用用户级技能。初始化用 project；本地/Pages/云端/AI 用 development 的对应指南；Android 用 android；服务失效只恢复对应 github/cloudbase/siliconflow。准备能力缺失交 env。本人不用补技术长提示。

按“已确认目标→现状复用→本轮实现方案→有序实施→助手验证→本人试用→记录接续”推进。确认过的 PRD/Canvas 直接用，不重走设计审批；小修复沿当前方案。助手按 docs/specs/_template.md 维护必要方案，技术文档不转为本人作业。

| 故障 | 下一步 | 禁止绕行 |
| --- | --- | --- |
| 引擎未开/容器停止 | 按 manifest 恢复现有引擎/连接与原 Compose，有界等待 | 宿主构建、换镜像、重装或重建作品 |
| 依赖/平台模块缺失 | 查锁文件、独立卷、镜像能力，同镜像修复 | 挂 Windows node_modules、临时升级主要版本 |
| 云端无权限 | 区分管理授权/应用会话/GRANT/RLS/资源归属 | anon全写、关闭RLS、前端管理员Key |
| 库未开通提示 | 识别实际 PG/NoSQL，核目标环境能力 | 默认买库、换库或新建替代环境 |
| APK内容旧 | 定位Web→sync→APK资源，重建核内容 | 只改文件名、交旧包、让本人反复安装排障 |

使用官方文档核实际 API/当前资格；发现与课程路线不同先核版本与适配依据，不能照示例更换技术架构。技术恢复在已有授权内连续执行；费用、本人身份、位置或确需改变已确认路线时说明具体影响。无法恢复记录阻塞，不能无界试验或将等待当成功。

实际配置与方案冲突时保留现有工程，查清差异并更新对应记录。技术方法在用户级Skill，项目事实在B，A只用于准备来源追溯；用户级方法更新不静默改变项目基线。

## 2.1 执行与 AI 设置

项目运行、依赖安装/锁文件更新、测试和恢复通过用户级 ai-coding-env/scripts/Invoke-CourseProject.ps1；Android沿 Build-Android.ps1、发布沿现有专用入口，均使用项目绑定镜像。依赖损坏读取环境技能 references/project-execution.md，在同镜像原卷恢复，不宿主编译或临时拉镜像。

仅明确选择案例后合并业务；用户 Skill 已安装不代表选择案例。开始按当前 Skill assets/course-timing.json 说明估时，长等待和超时说明真实原因，不虚报通过。

AI本人注册/优惠/充值决定与程序配置按通用开发 Skill implementation/ai-service-setup.md；P-01只落默认文件和配置路线，V4由本人在“设置 → AI 服务”输入Key和模型，秘密仅服务端存储。模型有效配置/revision两端共享。


2.1.1：先Test-CourseReadiness一次诊断；用Update-CourseProgress维护具名Spec和当前接续，等待分类记录。普通构建可显式-ReuseBuild按输入/产物摘要复用，但实际绑定/授权/线上内容仍核。方法读取通用development/implementation/efficient-execution.md，AI另读ai-settings-access.md。
