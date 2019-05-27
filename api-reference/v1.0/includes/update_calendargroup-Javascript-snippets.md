---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e0a1372f8f0fecfde1126b49b720dc073a805ed5
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34449710"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendarGroup = {
  name: "name-value"
};

let res = await client.api('/me/calendarGroups/{id}')
    .update({calendarGroup : calendarGroup});

```