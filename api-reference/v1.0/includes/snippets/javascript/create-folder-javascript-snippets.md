---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e8504d067845fd33dbcbc41d0c3f1fc834ad4867
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492212"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  name: "New Folder",
  folder: { },
  @microsoft.graph.conflictBehavior: "rename"
};

let res = await client.api('/me/drive/root/children')
    .post({driveItem : driveItem});

```