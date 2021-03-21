---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 580b720679b249df6d216963a6e5243ce60c0cc3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962739"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appliesTo = await client.api('/policies/tokenIssuancePolicies/{id}/appliesTo')
    .version('beta')
    .get();

```