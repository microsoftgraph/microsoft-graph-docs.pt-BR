---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 39f8ef72c43f05a63cfec568964ec6d46ae950c2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951263"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let resources = await client.api('/education/classes/{id}/assignments/{id}/submissions/{id}/resources')
    .version('beta')
    .get();

```