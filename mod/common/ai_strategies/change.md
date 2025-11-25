# AI Strategy Changes

- Removed `manowars` and `ironclads` from the default `goods_stances` override so the AI no longer prioritises those navies.
- Added new `goods_stances` entries for `newspapers`, `pharmaceuticals`, and `books` with appropriate research/building triggers.
- Set `treaty_port_value = 0` in both the default strategy and `ai_strategy_economic_imperialism`, and stripped treaty-port wargoal weight from `ai_strategy_colonial_expansion` to stop treaty port targeting.
