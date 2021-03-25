---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ba6b7780c019877caf38b109fbec9f718da49d69
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201148"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appConsentRequests = await client.api('/identityGovernance/appConsent/appConsentRequests')
    .version('beta')
    .filter('userConsentRequests/any (u:u/status eq \'InProgress\')')
    .get();

```