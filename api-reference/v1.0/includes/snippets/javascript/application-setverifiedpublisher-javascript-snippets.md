---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ed9dd5c5fda12366c3e86704792e18f6e1c519f5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810309"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const setVerifiedPublisher = {
    verifiedPublisherId: '1234567'
};

await client.api('/applications/{id}/setVerifiedPublisher')
    .post(setVerifiedPublisher);

```