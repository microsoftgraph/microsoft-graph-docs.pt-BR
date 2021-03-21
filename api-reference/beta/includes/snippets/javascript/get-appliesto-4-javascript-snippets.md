---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9b998316cf1d75936b24a8604ec667eabb022305
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962145"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appliesTo = await client.api('/policies/tokenLifetimePolicies/{id}/appliesTo')
    .version('beta')
    .get();

```