---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5418e1b56cc93534922125e82701253e73f16ab7
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48317965"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const todoTaskList = {
  displayName: "Travel items"
};

let res = await client.api('/me/todo/lists')
    .version('beta')
    .post(todoTaskList);

```