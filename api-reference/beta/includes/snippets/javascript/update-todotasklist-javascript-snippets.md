---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 55ed2bf32e46a3638beaf382abcfea383e46af04
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/16/2020
ms.locfileid: "47842985"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const todoTaskList = {
  displayName: "Vacation Plan",
};

let res = await client.api('/me/todo/lists/AAMkADIyAAAhrbPWAAA=')
    .version('beta')
    .update(todoTaskList);

```