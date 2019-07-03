---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 457e260cd2a8bec69b983097ed2f2ebff2f24663
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492627"
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