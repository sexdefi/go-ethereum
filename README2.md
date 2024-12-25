clique新增配置

```go
type CliqueConfig struct {
    Period         uint64          `json:"period"`         // Number of seconds between blocks to enforce
    Epoch          uint64          `json:"epoch"`          // Epoch length to reset votes and checkpoint
    BlockReward    *big.Int        `json:"blockReward"`    // Block reward for mining
    RewardAddress  *common.Address `json:"rewardAddress"`  // Address to receive block rewards
    MaxRewardBlock uint64          `json:"maxRewardBlock"` // Maximum block number that can receive block rewards
}