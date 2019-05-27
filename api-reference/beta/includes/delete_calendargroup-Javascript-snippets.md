---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 735477a1c584483fe940b60f40fd0f62b86c0744
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34438774"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendarGroups/{id}')
    .version('beta')
    .delete();

```