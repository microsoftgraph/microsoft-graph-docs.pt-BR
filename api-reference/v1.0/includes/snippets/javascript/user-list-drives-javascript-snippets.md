---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b0603466429547d504e296fbd7d6061b96d6ae67
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736161"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{userId}/drives')
    .get();

```