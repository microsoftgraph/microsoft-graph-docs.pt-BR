---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8823dc6d24a582dbd0245cdf0082ab590ed1b80e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773099"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let legalHold = await client.api('/compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}')
    .version('beta')
    .get();

```