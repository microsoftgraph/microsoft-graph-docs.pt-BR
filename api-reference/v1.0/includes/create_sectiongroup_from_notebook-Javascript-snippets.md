---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1469b5cdfd19975e0c9c9de313fb0f1428c0d60d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34460029"
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