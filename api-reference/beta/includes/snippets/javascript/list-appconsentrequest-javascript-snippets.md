---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 494865289f4e1dd5e45f771b279d38428fd7f893
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201147"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appConsentRequests = await client.api('/identityGovernance/appConsent/appConsentRequests')
    .version('beta')
    .get();

```