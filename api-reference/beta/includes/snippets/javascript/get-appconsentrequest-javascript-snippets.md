---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 729649e6e058754774a8de22762335fe0c2aba9b
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201714"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appConsentRequest = await client.api('/identityGovernance/appConsent/appConsentRequests/af330b30-dd59-4482-a848-0fd81b0438ed')
    .version('beta')
    .get();

```