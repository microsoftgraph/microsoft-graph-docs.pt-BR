---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a6400fc54ad13736ebe67b98c4e59ecad030acfb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953212"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let rosterPlans = await client.api('/users/{usersId}/planner/rosterPlans')
    .version('beta')
    .get();

```