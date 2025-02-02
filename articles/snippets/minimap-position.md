# Minimap Position

You can modify the minimap position with alt:V internal function.

`T` - Top \
`B` - Bottom \
`R` - Right \
`L` - Left

```js
import { setMinimapComponentPosition } from 'alt-client';

// Player + Compass + HP
setMinimapComponentPosition('minimap', 'L', 'B', 0.811, -0.768, 0.150, 0.188888);
// Purple Route
setMinimapComponentPosition('minimap_mask', 'L', 'B', 0.8355, -0.738, 0.111, 0.159);
// Map
setMinimapComponentPosition('minimap_blur', 'L', 'B', 0.7855, -0.748, 0.266, 0.237);
```

To see the new position you have to open the Pause Menu with `Esc` key or use the below snippet. \
If you find a better way, you can send a pull request to GitHub.

```js
import { hash } from 'alt-client';
import { restartFrontendMenu } from 'natives';

restartFrontendMenu(hash('FE_MENU_VERSION_MP_PAUSE'), -1);
```

# Used APIs

- [setMinimapComponentPosition](https://docs.altv.mp/js/api/alt-client.html#_altmp_altv_types_alt_client_setMinimapComponentPosition_1)
- [hash](https://docs.altv.mp/js/api/alt-client.html#_altmp_altv_types_alt_client_hash)
- [restartFrontendMenu](https://natives.altv.mp/#/0x10706DC6AD2D49C0)
