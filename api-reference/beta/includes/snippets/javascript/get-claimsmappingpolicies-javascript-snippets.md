---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 02effa2234416fe972924eb36e327656fa37ccac
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801446"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let claimsMappingPolicies = await client.api('/policies/claimsMappingPolicies')
    .version('beta')
    .get();

```