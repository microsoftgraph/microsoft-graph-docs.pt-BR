---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ab828ba704d76b61c02c75dbd75955e86a4021d8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802790"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const removeKey = {
    keyId: 'f0b0b335-1d71-4883-8f98-567911bfdca6',
    proof: 'eyJ0eXAiOiJ...'
};

await client.api('/applications/{id}/removeKey')
    .post(removeKey);

```