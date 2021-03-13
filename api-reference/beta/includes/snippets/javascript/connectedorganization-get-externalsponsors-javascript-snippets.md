---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5be99baa9f625641e665567a522eeb907011f52f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790617"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let externalSponsors = await client.api('/identityGovernance/entitlementManagement/connectedOrganizations/{id}/externalSponsors')
    .version('beta')
    .get();

```