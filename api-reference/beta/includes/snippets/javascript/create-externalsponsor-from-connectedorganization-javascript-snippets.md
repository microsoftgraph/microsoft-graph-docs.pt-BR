---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f1ae97408daff68bba1f9461e717314ed67aee230093bea3aa0c92e5f8b39a01
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100507"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id': 'https://graph.microsoft.com/beta/users/{id}'
};

await client.api('/identityGovernance/entitlementManagement/connectedOrganizations/{id}/externalSponsors/$ref')
    .version('beta')
    .post(directoryObject);

```