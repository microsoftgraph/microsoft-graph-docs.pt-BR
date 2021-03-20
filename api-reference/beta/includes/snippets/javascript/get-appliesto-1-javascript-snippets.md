---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 45aa558c02fcd5ddbd739a7d51718be56b844b34
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947678"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appliesTo = await client.api('/policies/claimsMappingPolicies/{id}/appliesTo')
    .version('beta')
    .get();

```