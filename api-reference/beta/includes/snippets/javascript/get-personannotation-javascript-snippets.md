---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b12a12a5681d08fdea692f2ad981d5a9fba9b942
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809784"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let personAnnotation = await client.api('/me/profile/notes/{id}')
    .version('beta')
    .get();

```