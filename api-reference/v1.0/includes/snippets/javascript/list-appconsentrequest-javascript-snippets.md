---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 86ce77e95d7ee0d3bfd103f232d886213f8aa96f
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508176"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appConsentRequests = await client.api('/identityGovernance/appConsent/appConsentRequests')
    .get();

```