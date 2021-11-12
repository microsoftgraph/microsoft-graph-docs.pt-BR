---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d6b91114b569761746e394c7d6800a11a2aa5b9c4f062cf58a308e10baf2cdf6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157922"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const groupLifecyclePolicy = {
  groupLifetimeInDays: 100,
  managedGroupTypes: 'Selected',
  alternateNotificationEmails: 'admin@contoso.com'
};

await client.api('/groupLifecyclePolicies')
    .version('beta')
    .post(groupLifecyclePolicy);

```