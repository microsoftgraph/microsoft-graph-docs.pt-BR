---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b381b0dfc2a611c36e4bf3a7c28121db0a187902
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787663"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let definitions = await client.api('/identityGovernance/accessReviews/definitions')
    .version('beta')
    .skip(0)
    .top(100)
    .get();

```