---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 24603a6ccb10b10e62bb1f0394ae51a354fc43ab6da082f1e70e5750b4fe1225
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100538"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/entitlementManagement/connectedOrganizations/{connectedOrganizationId}/externalSponsors/{id}/$ref')
    .version('beta')
    .delete();

```