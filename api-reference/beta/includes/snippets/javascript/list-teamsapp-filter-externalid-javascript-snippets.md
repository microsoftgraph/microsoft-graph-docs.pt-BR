---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 35d9673ee2c45b091f3b36f2500646c09f675b70
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801886"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamsApps = await client.api('/appCatalogs/teamsApps')
    .version('beta')
    .filter('externalId eq \'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee\'')
    .get();

```