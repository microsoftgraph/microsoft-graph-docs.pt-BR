---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bf4a7858fc0fe1d2e0b77ee483b786a3c799a27c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795748"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let oAuth2PermissionGrant = await client.api('/oauth2PermissionGrants/{id}')
    .get();

```