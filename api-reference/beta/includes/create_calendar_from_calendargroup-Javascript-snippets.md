---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 56d8c90693b3b2b1c828d7e381b4ddab079fee9b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34434375"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendar = {
  name: "name-value",
  color: {
  }
};

let res = await client.api('/me/calendarGroups/{id}/calendars')
    .version('beta')
    .post({calendar : calendar});

```