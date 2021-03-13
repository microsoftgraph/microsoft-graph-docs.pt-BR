---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d49df44c8aa29154a290f7d0934db7e9d803cd6e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780174"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/servicePrincipals/{id}/claimsMappingPolicies/{id}/$ref')
    .version('beta')
    .delete();

```