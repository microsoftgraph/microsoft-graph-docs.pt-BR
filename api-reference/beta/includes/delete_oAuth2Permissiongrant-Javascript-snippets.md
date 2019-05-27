---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f2902928dbc2e75b6319a76488d6252e53cb9437
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437997"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/oAuth2Permissiongrants/{id}')
    .version('beta')
    .delete();

```