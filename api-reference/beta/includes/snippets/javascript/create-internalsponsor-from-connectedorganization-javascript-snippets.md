---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6d3224b38efa3f4f6addc1d9d6bc626cca85c011
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810111"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  @odata.id: "https://graph.microsoft.com/beta/users/{id}"
};

let res = await client.api('/identityGovernance/entitlementManagement/connectedOrganizations/{id}/internalSponsors/$ref')
    .version('beta')
    .post(directoryObject);

```