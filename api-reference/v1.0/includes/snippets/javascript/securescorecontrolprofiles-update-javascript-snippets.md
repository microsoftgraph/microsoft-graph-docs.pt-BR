---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5d84a9c2ad3e700dbe9eb04a35ecb97f9daf42d0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796892"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const secureScoreControlProfile = {
  assignedTo: '',
  comment: 'control is reviewed',
  state: 'Reviewed',
  vendorInformation: {
    provider: 'SecureScore',
    providerVersion: null,
    subProvider: null,
    vendor: 'Microsoft'
  }
};

await client.api('/security/secureScoreControlProfiles/NonOwnerAccess')
    .update(secureScoreControlProfile);

```