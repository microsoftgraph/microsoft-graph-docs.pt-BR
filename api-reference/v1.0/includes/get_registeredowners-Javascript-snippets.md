---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 83f44945f15bf60c136df37742f2cc8d614c20d8
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34477317"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/devices/{id}/registeredOwners')
    .get();

```