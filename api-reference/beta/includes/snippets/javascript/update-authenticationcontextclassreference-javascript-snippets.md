---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5d9696ff926c83a3df3ab684397af6a82cb3dc475fc2431f736c1b7e43a70c7c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898870"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authenticationContextClassReference = {
   value: 
    [
      {
         displayName: 'Contoso trusted locations',
        description: 'Access is only allowed from trusted locations',
        isAvailable: true
      }
    ]
};

await client.api('/identity/conditionalAccess/authenticationContextClassReferences/c1')
    .version('beta')
    .update(authenticationContextClassReference);

```