---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 457e260cd2a8bec69b983097ed2f2ebff2f24663
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722961"
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