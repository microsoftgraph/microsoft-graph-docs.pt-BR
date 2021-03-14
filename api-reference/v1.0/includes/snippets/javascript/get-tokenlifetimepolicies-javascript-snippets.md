---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 300fe00c9409155259e26d1d38514a7e1d6e3190
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809152"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tokenLifetimePolicies = await client.api('/policies/tokenLifetimePolicies')
    .get();

```