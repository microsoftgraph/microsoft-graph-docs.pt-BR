---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ba1c836c9b6e1d07cba1e39d560f3ab2884c8ff2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776715"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let legalHolds = await client.api('/compliance/ediscovery/cases/{caseId}/legalHolds')
    .version('beta')
    .get();

```