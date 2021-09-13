---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 014bc60ec8bd062e2d1989ad1b3e60587cdcd9f137c2bcde231a96c82e84f5cd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329134"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userConsentRequests = await client.api('/identityGovernance/appConsent/appConsentRequests/ee245379-e3bb-4944-a997-24115f0b8b5e/userConsentRequests')
    .get();

```