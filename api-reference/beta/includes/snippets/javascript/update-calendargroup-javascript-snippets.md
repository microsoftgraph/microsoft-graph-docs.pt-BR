---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 241ed1161767c547ef21f543732a59ca7f4144bb
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709058"
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
    .version('beta')
    .update({calendarGroup : calendarGroup});

```