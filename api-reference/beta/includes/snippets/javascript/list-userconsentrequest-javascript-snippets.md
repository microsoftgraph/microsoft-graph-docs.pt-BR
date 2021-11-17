---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e766f428ad8e71098e48656b3962305bd8bc62fa1dd505c84c689259a69dcbad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216832"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userConsentRequests = await client.api('/identityGovernance/appConsent/appConsentRequests/ee245379-e3bb-4944-a997-24115f0b8b5e/userConsentRequests')
    .version('beta')
    .get();

```