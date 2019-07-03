---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b0603466429547d504e296fbd7d6061b96d6ae67
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35507450"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{userId}/drives')
    .get();

```