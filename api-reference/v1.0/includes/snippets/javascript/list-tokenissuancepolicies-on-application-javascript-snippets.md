---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b79e981967538ab36c7f69745a6bf444a585d1af
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800902"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tokenIssuancePolicies = await client.api('/applications/{id}/tokenIssuancePolicies')
    .get();

```