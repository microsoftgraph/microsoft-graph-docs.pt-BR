---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1469b5cdfd19975e0c9c9de313fb0f1428c0d60d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730059"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sectionGroup = {
  displayName: "Section group name"
};

let res = await client.api('/me/onenote/notebooks/{id}/sectionGroups')
    .post({sectionGroup : sectionGroup});

```