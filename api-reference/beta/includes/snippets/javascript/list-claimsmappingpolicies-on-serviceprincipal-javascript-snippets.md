---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 817e2ac20f241618d321f0587670835f59726798
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2020
ms.locfileid: "41558797"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/claimsMappingPolicies')
    .version('beta')
    .get();

```