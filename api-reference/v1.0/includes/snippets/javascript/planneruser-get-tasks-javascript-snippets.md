---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 468bc0acd88fc972502cd3243b6bc12e07ea7608d61cafc11e7cd8052b148ce4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57376795"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tasks = await client.api('/me/planner/tasks')
    .get();

```