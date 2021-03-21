---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e79fe78b9a287dec6cf2885eca6f51ab31638c30
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959366"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appliesTo = await client.api('/policies/tokenIssuancePolicies/{id}/appliesTo')
    .get();

```