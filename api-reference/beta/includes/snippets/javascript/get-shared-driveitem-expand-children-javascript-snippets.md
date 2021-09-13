---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b8de454c8690e7274f026d9f4f74918fcd7495ba28211b949848954fe1b398ef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327796"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let driveItem = await client.api('/shares/{shareIdOrUrl}/driveItem')
    .version('beta')
    .expand('children')
    .get();

```