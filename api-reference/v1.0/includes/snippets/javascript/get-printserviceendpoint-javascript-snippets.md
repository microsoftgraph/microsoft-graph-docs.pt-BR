---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 29019433b21f72cbe701416fde5e60cbe25203fd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777542"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printServiceEndpoint = await client.api('/print/services/{printServiceId}/endpoints/{printServiceEndpointId}')
    .get();

```