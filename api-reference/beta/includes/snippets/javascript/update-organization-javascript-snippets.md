---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7f508b1a39d5da4918d61e4df546536b2f0d78bc
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323332"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const organization = {
  marketingNotificationEmails: ['marketing@contoso.com'],
  privacyProfile: 
    {
      contactEmail: 'alice@contoso.com',
      statementUrl: 'https://contoso.com/privacyStatement'
    },
  securityComplianceNotificationMails: ['security@contoso.com'],
  securityComplianceNotificationPhones: ['(123) 456-7890'],
  technicalNotificationMails: ['tech@contoso.com']
};

await client.api('/organization/84841066-274d-4ec0-a5c1-276be684bdd3')
    .version('beta')
    .update(organization);

```