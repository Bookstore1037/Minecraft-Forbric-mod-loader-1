# Forbric nightly 2026-10-06: FAIL

| | |
| --- | --- |
| commit | [`520d7aad11cc`](https://github.com/Ray-T-r/Minecraft-Forbric-mod-loader/commit/520d7aad11cc7c9b8c8278b5f541e4429e1f7623) Describe the writeByte repair and ThinnedCallOrdinals |
| tested | `origin/main` on the developer's Mac (commit status `nightly/dev-mac`) |
| started | 2026-10-06 02:30 +0800 |
| soak (`gate-m34-soak.sh`) | skipped: it runs on Sundays |
| integration | FAILED (exit 1) in 3 min |
| gates | TIMED OUT after 180 min (limit 180 min): no RESULT lines |

## Integration: `python3 tools/dev.py integration`

### JUnit totals

| suite | tests | executed | skipped | skip % | failed |
| --- | ---: | ---: | ---: | ---: | ---: |
| test | 3668 | 3668 | 0 | 0.0 | 6 |

Did not execute (no results): `transferTest`

**Failed (6):**
- `test` net.forbric.kernel.boot.KernelBundledMixinExtrasStagedTest.[1] true (org.opentest4j.AssertionFailedError)
- `test` net.forbric.kernel.boot.KernelBundledMixinExtrasStagedTest.[2] false (org.opentest4j.AssertionFailedError)
- `test` net.forbric.kernel.mixin.MixinRetargetRenamedBodyCorpusTest.r3MovesExactlyThePinnedInjectorsOverTheAuditCorpus() (org.opentest4j.AssertionFailedError)
- `test` net.forbric.kernel.mixin.MixinTwinRebindTest.releasedLiquidBounceMovesItsFaceTestAndNothingElse() (org.opentest4j.AssertionFailedError)
- `test` net.forbric.kernel.mixin.ReplacedCallRedirectsTest.releasedViaFabricPlusMovesItsThreeRedirects() (org.opentest4j.AssertionFailedError)
- `test` net.forbric.kernel.mixin.ThinnedCallOrdinalsTest.releasedViaFabricPlusCountsOnTheMergedBody() (org.opentest4j.AssertionFailedError)

## Gates: `bash forbric-kernel/run/compat/gates-all.sh -j auto --skip gate-m34-soak.sh`

_No `forbric-kernel/build/gates/summary.txt`: the run stopped before any gate reported._

Logs stay on the Mac, in the nightly worktree: `build/nightly/` and `forbric-kernel/build/gates/`.
