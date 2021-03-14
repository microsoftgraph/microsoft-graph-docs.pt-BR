---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e1e04e33a8008cf23acc0e8d8b5e26b5e43a2bf4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802873"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/applications/{id}/tokenLifetimePolicies/{id}/$ref')
    .delete();

```