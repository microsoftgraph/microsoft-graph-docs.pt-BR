---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 52510d14314f723441a13f41f8368d90368cc77e
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/16/2020
ms.locfileid: "47843125"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const todoTaskList = {
  displayName: "Travel items",
};

let res = await client.api('/me/todo/lists')
    .version('beta')
    .post(todoTaskList);

```