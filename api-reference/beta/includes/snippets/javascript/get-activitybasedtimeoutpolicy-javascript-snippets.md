---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: da3df5982d3125a4a91efbecde9ad85a75655e66
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2020
ms.locfileid: "41475514"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/activityBasedTimeoutPolicies/{id}')
    .version('beta')
    .get();

```