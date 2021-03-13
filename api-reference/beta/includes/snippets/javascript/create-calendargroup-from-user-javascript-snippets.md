---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1aee90c9c984b9c461ef903bead0ee50eda76ba6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781153"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendarGroup = {
  name: 'name-value',
  classId: 'classId-value',
  changeKey: 'changeKey-value'
};

await client.api('/me/calendarGroups')
    .version('beta')
    .post(calendarGroup);

```