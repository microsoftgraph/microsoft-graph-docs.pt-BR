---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c6fad1ad1cebe3c5f13cb694603e03ab8d3672bb
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51572985"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterByCurrentUser = await client.api('/identityGovernance/appConsent/appConsentRequests/filterByCurrentUser(on='reviewer')')
    .version('beta')
    .filter('userConsentRequests/any(u:u/status eq \'InProgress\')')
    .get();

```