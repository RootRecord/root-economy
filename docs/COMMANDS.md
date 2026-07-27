# Commands and permissions

## Commands

| Command | Description | Permission | Usage |
|---------|-------------|------------|-------|
| `/balance` | Show balance | `` | `/balance` |
| `/pay` | Pay another player or donate to the Server Reserve | `` | `/<command> <player/reserve> <amount> / /<command> reserve confirm/cancel` |
| `/paytoggle` | Toggle accepting payments | `` | `/paytoggle` |
| `/baltop` | Balance leaderboard (players; towns/nations on Towny) | `` | `/<command> [players/towns/nations]` |
| `/reserve` | Server treasury reserve stats (balance, inflows/outflows, playtime) | `` | `/reserve` |
| `/totals` | Precomputed economy list totals (entry types, Towny intake, supply, pools) | `` | `/totals` |
| `/economy` | Total economy (Notes vs gold mined), inflation pressure, and tax info | `` | `/economy` |
| `/tax` | Live transaction tax rate (dynamic while Notes are over-issued) | `` | `/tax` |
| `/mint` | Convert gold items to G, or withdraw G as gold items | `` | `/<command> <hand/all/gold> [amount/max]` |
| `/grant` | Grant G from treasury to a player (logged) | `rootessentials.grant` | `/<command> <player> <amount> [reason]` |
| `/bonds` | Bond vault â€” issue bonds, collect compounding yield, redeem notes in full | `` | `/<command> [create <amount/root>/merge]` |
| `/rootbonds` | Admin reload for Root-Bonds | `rootbonds.reload` | `/<command> reload` |
| `/loan` | Borrow, view, or repay a personal loan | `` | `/<command> <take/info/repay/list> [amount]` |
| `/townloan` | Mayor â€” borrow from Server Reserve into town bank, or repay | `` | `/<command> <take/repay/info/list> [amount]` |
| `/rootloans` | Admin reload for Root-Loans | `rootloans.reload` | `/<command> reload` |
| `/rootupkeep` | Admin controls for inactivity tax | `rootupkeep.admin` | `/<command> reload/run` |

## Permissions

| Permission | Description | Default |
|------------|-------------|---------|
| `rootbonds.use` | Open /bonds and issue bonds via GUI | `true` |
| `rootbonds.reload` | Reload root-bonds.yml | `op` |
| `rootloans.use` | Use /loan take, info, and repay | `true` |
| `rootloans.town.use` | Mayor use /townloan | `true` |
| `rootloans.list` | View all active personal loans | `op` |
| `rootloans.town.list` | View all active town loans | `op` |
| `rootloans.reload` | Reload root-loans.yml | `op` |
| `rootupkeep.admin` | Reload config and manually trigger inactivity tax | `op` |
| `rootessentials.balance` | Use /balance and /bal | `true` |
| `essentials.balance` | EssentialsX alias for /balance | `true` |
| `rootessentials.pay` | Use /pay | `true` |
| `essentials.pay` | EssentialsX alias for /pay | `true` |
| `rootessentials.paytoggle` | Use /paytoggle | `true` |
| `essentials.paytoggle` | EssentialsX alias for /paytoggle | `true` |
| `rootessentials.mint` | Use /mint | `true` |
| `essentials.mint` | EssentialsX alias for /mint | `true` |
| `rootessentials.reserve` | View server reserve stats (read-only) | `true` |
| `rootessentials.totals` | View precomputed economy list totals (read-only) | `true` |
| `rootessentials.economy` | View total economy (Notes vs gold mined) and inflation pressure (read-only) | `true` |
| `rootessentials.tax` | View live transaction tax rate (read-only) | `true` |
| `rootessentials.baltop` | Balance leaderboards (read-only) | `true` |
| `essentials.baltop` | EssentialsX alias for /baltop | `true` |
| `rootessentials.grant` | Grant G from treasury to a player | `op` |
| `rootmc.grant` | Grant G from treasury (wiki alias for rootessentials.grant) | `op` |

