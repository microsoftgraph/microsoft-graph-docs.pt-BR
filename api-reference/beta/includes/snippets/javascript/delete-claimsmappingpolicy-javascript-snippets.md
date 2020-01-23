---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 99e4ca07dab10f2a468f826b69c5dd3fafd59901
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2020
ms.locfileid: "41476278"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/claimsMappingPolicies/{id}')
    .version('beta')
    .delete();

```