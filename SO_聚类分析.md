# SO 变更原因聚类分析（相对 AOSP12）

- 数据来源：`/home/runner/work/mute_unmute/mute_unmute/audio_ROM.xlsx`
- 统计口径：仅统计 `.so`，共 **166** 个条目（含 32/64 位及 system/vendor 变体）
- 说明：同一 SO 可能具备多重属性；为便于汇总，本报告按“主导原因”单类归档。

## 聚类总览

| 类别 | 数量 |
|---|---:|
| 功能增强 | 66 |
| HIDL 向 AIDL 迁移 | 52 |
| 音频框架拆分更细 | 9 |
| 策略与配置体系增强 | 30 |
| 权限与稳定性要求提升 | 9 |

## 功能增强（66）

| SO 路径 | 归类依据 |
|---|---|
| `/system/lib/libaaudio.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib/libaaudio_internal.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib/libaudio-resampler.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib/libaudioclient.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib/libaudioeffect_jni.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib/libaudiohal.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib/libaudiohal@6.0.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib/libaudiohal@7.0.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib/libaudiohal@7.1.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib/libaudiohal@local.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib/libaudioroute.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib/libaudiospdif.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib/libaudioutils.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib/libhwmediamonitor_client.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib/libnbaio.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib/libsoundpool.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib/libstagefright_amrnb_common.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib/libstagefright_bufferpool@2.0.1.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib/libwilhelm.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libaaudio.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libaaudio_internal.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libaudioalgoservice_jni.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libaudioclient.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libaudioeffect_jni.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libaudioflinger.huawei.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libaudioflinger.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libaudiohal.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libaudiohal@6.0.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libaudiohal@7.0.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libaudiohal@7.1.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libaudiohal@local.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libaudioroute.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libaudiospdif.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libaudioutils.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libcodec2_hidl_plugin_stub.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libcodec2_soft_apvdec.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libcodec2_soft_apvenc.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libcodec2_soft_av1dec_dav1d.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libcodec2_soft_av1dec_gav1.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libcodec2_soft_av1enc.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libcodec2_soft_flacdec.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libcodec2_soft_flacenc.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libcodec2_soft_g711alawdec.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libcodec2_soft_g711mlawdec.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libcodec2_soft_h263enc.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libcodec2_soft_mpeg4enc.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libcodec2_soft_opusdec.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libcodec2_soft_vorbisdec.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libcodec2_soft_vp8dec.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libcodec2_soft_vp8enc.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libcodec2_soft_vp9dec.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libcodec2_soft_vp9enc.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libheadtracking-binding.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libheadtracking.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libmedia_codecserviceregistrant.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libnbaio.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libsounddose.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libsoundpool.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libstagefright_bufferpool@2.0.1.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/system/lib64/libwilhelm.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/vendor/lib/libaudioutils.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/vendor/lib/libmediautils_vendor.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/vendor/lib/soundfx/libhapticgenerator.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/vendor/lib64/libaudioutils.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/vendor/lib64/libmediautils_vendor.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |
| `/vendor/lib64/soundfx/libhapticgenerator.so` | 未命中前述基础设施关键词，归入能力增强（含编解码、空间音频、效果链等） |

## HIDL 向 AIDL 迁移（52）

| SO 路径 | 归类依据 |
|---|---|
| `/system/lib/aaudio-aidl-cpp.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib/android.media.audio.common.types-V1-ndk.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib/android.media.audio.common.types-V4-cpp.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib/android.media.audio.common.types-V4-ndk.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib/android.media.audio.eraser.types-V1-ndk.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib/audio-permission-aidl-cpp.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib/audioclient-types-aidl-cpp.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib/audioflinger-aidl-cpp.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib/audiopolicy-aidl-cpp.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib/audiopolicy-types-aidl-cpp.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib/av-audio-types-aidl-ndk.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib/av-types-aidl-cpp.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib/capture_state_listener-aidl-cpp.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib/effect-aidl-cpp.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib/graphicbuffersource-aidl-ndk.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib/libaudio_aidl_conversion_common_cpp.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib/libaudio_aidl_conversion_common_ndk.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib/libaudio_aidl_conversion_common_ndk_cpp.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib/libaudio_aidl_conversion_core_ndk.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib/libaudio_aidl_conversion_effect_ndk.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib/libaudioaidlcommon.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib/libaudioclient_aidl_conversion.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib/libaudiohal@aidl.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib/libstagefright_graphicbuffersource_aidl.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib/media_quality_aidl_interface-cpp.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib/mediametricsservice-aidl-cpp.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib64/aaudio-aidl-cpp.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib64/android.media.audio.common.types-V1-ndk.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib64/android.media.audio.common.types-V4-cpp.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib64/android.media.audio.common.types-V4-ndk.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib64/android.media.audio.eraser.types-V1-ndk.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib64/audio-permission-aidl-cpp.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib64/audioclient-types-aidl-cpp.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib64/audioflinger-aidl-cpp.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib64/audiopolicy-aidl-cpp.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib64/audiopolicy-types-aidl-cpp.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib64/av-audio-types-aidl-ndk.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib64/av-types-aidl-cpp.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib64/capture_state_listener-aidl-cpp.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib64/effect-aidl-cpp.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib64/graphicbuffersource-aidl-ndk.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib64/libaudio_aidl_conversion_common_cpp.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib64/libaudio_aidl_conversion_common_ndk.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib64/libaudio_aidl_conversion_common_ndk_cpp.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib64/libaudio_aidl_conversion_core_ndk.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib64/libaudio_aidl_conversion_effect_ndk.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib64/libaudioaidlcommon.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib64/libaudioclient_aidl_conversion.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib64/libaudiohal@aidl.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib64/libstagefright_graphicbuffersource_aidl.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib64/media_quality_aidl_interface-cpp.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |
| `/system/lib64/mediametricsservice-aidl-cpp.so` | 命中 AIDL/类型接口命名（aidl、types-V*、audiohal@aidl） |

## 音频框架拆分更细（9）

| SO 路径 | 归类依据 |
|---|---|
| `/system/lib/libaudiodatadump.so` | 命中框架子模块拆分命名（fastpath/datapath/utils/timing/components 等） |
| `/system/lib/libaudiofoundation.so` | 命中框架子模块拆分命名（fastpath/datapath/utils/timing/components 等） |
| `/system/lib64/libaudiodatadump.so` | 命中框架子模块拆分命名（fastpath/datapath/utils/timing/components 等） |
| `/system/lib64/libaudioflinger_datapath.so` | 命中框架子模块拆分命名（fastpath/datapath/utils/timing/components 等） |
| `/system/lib64/libaudioflinger_fastpath.so` | 命中框架子模块拆分命名（fastpath/datapath/utils/timing/components 等） |
| `/system/lib64/libaudioflinger_timing.so` | 命中框架子模块拆分命名（fastpath/datapath/utils/timing/components 等） |
| `/system/lib64/libaudioflinger_utils.so` | 命中框架子模块拆分命名（fastpath/datapath/utils/timing/components 等） |
| `/system/lib64/libaudiofoundation.so` | 命中框架子模块拆分命名（fastpath/datapath/utils/timing/components 等） |
| `/system/lib64/libaudiousecasevalidation.so` | 命中框架子模块拆分命名（fastpath/datapath/utils/timing/components 等） |

## 策略与配置体系增强（30）

| SO 路径 | 归类依据 |
|---|---|
| `/system/lib/aconfig_mediacodec_flags_c_lib.so` | 命中策略/配置关键词（audiopolicy、aconfig、effectsconfig） |
| `/system/lib/android.media.audio-aconfig-cc.so` | 命中策略/配置关键词（audiopolicy、aconfig、effectsconfig） |
| `/system/lib/android.media.audiopolicy-aconfig-cc.so` | 命中策略/配置关键词（audiopolicy、aconfig、effectsconfig） |
| `/system/lib/com.android.media.aaudio-aconfig-cc.so` | 命中策略/配置关键词（audiopolicy、aconfig、effectsconfig） |
| `/system/lib/com.android.media.audio-aconfig-cc.so` | 命中策略/配置关键词（audiopolicy、aconfig、effectsconfig） |
| `/system/lib/com.android.media.audioclient-aconfig-cc.so` | 命中策略/配置关键词（audiopolicy、aconfig、effectsconfig） |
| `/system/lib/com.android.media.audioserver-aconfig-cc.so` | 命中策略/配置关键词（audiopolicy、aconfig、effectsconfig） |
| `/system/lib/libaudiopolicy.so` | 命中策略/配置关键词（audiopolicy、aconfig、effectsconfig） |
| `/system/lib/libaudiopolicycomponents.so` | 命中策略/配置关键词（audiopolicy、aconfig、effectsconfig） |
| `/system/lib/libaudiopolicyenginedefault.so` | 命中策略/配置关键词（audiopolicy、aconfig、effectsconfig） |
| `/system/lib/libaudiopolicymanager.huawei.so` | 命中策略/配置关键词（audiopolicy、aconfig、effectsconfig） |
| `/system/lib/libaudiopolicymanagerCust.huawei.so` | 命中策略/配置关键词（audiopolicy、aconfig、effectsconfig） |
| `/system/lib/libaudiopolicymanagerdefault.so` | 命中策略/配置关键词（audiopolicy、aconfig、effectsconfig） |
| `/system/lib/libeffectsconfig.so` | 命中策略/配置关键词（audiopolicy、aconfig、effectsconfig） |
| `/system/lib64/aconfig_mediacodec_flags_c_lib.so` | 命中策略/配置关键词（audiopolicy、aconfig、effectsconfig） |
| `/system/lib64/android.media.audio-aconfig-cc.so` | 命中策略/配置关键词（audiopolicy、aconfig、effectsconfig） |
| `/system/lib64/android.media.audiopolicy-aconfig-cc.so` | 命中策略/配置关键词（audiopolicy、aconfig、effectsconfig） |
| `/system/lib64/com.android.media.aaudio-aconfig-cc.so` | 命中策略/配置关键词（audiopolicy、aconfig、effectsconfig） |
| `/system/lib64/com.android.media.audio-aconfig-cc.so` | 命中策略/配置关键词（audiopolicy、aconfig、effectsconfig） |
| `/system/lib64/com.android.media.audioclient-aconfig-cc.so` | 命中策略/配置关键词（audiopolicy、aconfig、effectsconfig） |
| `/system/lib64/com.android.media.audioserver-aconfig-cc.so` | 命中策略/配置关键词（audiopolicy、aconfig、effectsconfig） |
| `/system/lib64/libaudiopolicy.so` | 命中策略/配置关键词（audiopolicy、aconfig、effectsconfig） |
| `/system/lib64/libaudiopolicycomponents.so` | 命中策略/配置关键词（audiopolicy、aconfig、effectsconfig） |
| `/system/lib64/libaudiopolicyenginedefault.so` | 命中策略/配置关键词（audiopolicy、aconfig、effectsconfig） |
| `/system/lib64/libaudiopolicymanager.huawei.so` | 命中策略/配置关键词（audiopolicy、aconfig、effectsconfig） |
| `/system/lib64/libaudiopolicymanagerdefault.so` | 命中策略/配置关键词（audiopolicy、aconfig、effectsconfig） |
| `/system/lib64/libaudiopolicyservice.so` | 命中策略/配置关键词（audiopolicy、aconfig、effectsconfig） |
| `/system/lib64/libeffectsconfig.so` | 命中策略/配置关键词（audiopolicy、aconfig、effectsconfig） |
| `/vendor/lib/libeffectsconfig.so` | 命中策略/配置关键词（audiopolicy、aconfig、effectsconfig） |
| `/vendor/lib64/libeffectsconfig.so` | 命中策略/配置关键词（audiopolicy、aconfig、effectsconfig） |

## 权限与稳定性要求提升（9）

| SO 路径 | 归类依据 |
|---|---|
| `/system/lib/libaudiohal_deathhandler.so` | 命中权限/稳定性关键词（permission、deathhandler、fmq、shmem） |
| `/system/lib/libshmemcompat.so` | 命中权限/稳定性关键词（permission、deathhandler、fmq、shmem） |
| `/system/lib/libshmemutil.so` | 命中权限/稳定性关键词（permission、deathhandler、fmq、shmem） |
| `/system/lib64/libaudiohal_deathhandler.so` | 命中权限/稳定性关键词（permission、deathhandler、fmq、shmem） |
| `/system/lib64/libfmq.so` | 命中权限/稳定性关键词（permission、deathhandler、fmq、shmem） |
| `/system/lib64/libresourcemanagerservice.so` | 命中权限/稳定性关键词（permission、deathhandler、fmq、shmem） |
| `/system/lib64/libshmemcompat.so` | 命中权限/稳定性关键词（permission、deathhandler、fmq、shmem） |
| `/vendor/lib/libfmq.so` | 命中权限/稳定性关键词（permission、deathhandler、fmq、shmem） |
| `/vendor/lib64/libfmq.so` | 命中权限/稳定性关键词（permission、deathhandler、fmq、shmem） |
