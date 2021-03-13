---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ae0821c7fc29feb1b99d034dec196c75dee695c0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772917"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const legalHold = {
  description: 'This is a description for a legalHold'
};

await client.api('/compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}')
    .version('beta')
    .update(legalHold);

```