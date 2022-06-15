---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 877312ad0890bb9e8f097e4d91e807ce1c32cfef2fcfaa86324f0f57d7409618
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100530"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/entitlementManagement/connectedOrganizations/{connectedOrganizationId}/internalSponsors/{id}/$ref')
    .version('beta')
    .delete();

```