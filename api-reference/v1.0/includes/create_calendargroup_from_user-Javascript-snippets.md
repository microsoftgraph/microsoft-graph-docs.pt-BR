---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 457e260cd2a8bec69b983097ed2f2ebff2f24663
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34455888"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendarGroup = {
  name: "name-value",
  classId: "classId-value",
  changeKey: "changeKey-value"
};

let res = await client.api('/me/calendarGroups')
    .post({calendarGroup : calendarGroup});

```