---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 390c29df69c589f0a63bf2eb82a32f26d73290f1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794730"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/synchronizationProfiles/{id}/start')
    .version('beta')
    .post();

```