---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6d01695cb89989f012551be00ef8c015841df12c
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/07/2020
ms.locfileid: "48375723"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const todoTaskList = {
  displayName: "Vacation Plan"
};

let res = await client.api('/me/todo/lists/AAMkADIyAAAhrbPWAAA=')
    .version('beta')
    .update(todoTaskList);

```