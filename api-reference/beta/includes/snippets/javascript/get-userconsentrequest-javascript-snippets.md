---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bebd9cf3d1f4f800939a1ffafc2dbe923a0b29a0
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201882"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userConsentRequest = await client.api('/identityGovernance/appConsent/appConsentRequests/ee245379-e3bb-4944-a997-24115f0b8b5e/userConsentRequests/acef2660-d194-4943-b927-4fe4fb5cb7e3')
    .version('beta')
    .get();

```