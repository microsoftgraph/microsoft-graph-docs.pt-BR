---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 30d6fd12ad2df43c478e783face8f6ea3895406e
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59764738"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const invitation = {
  invitedUserEmailAddress: 'admin@fabrikam.com',
  inviteRedirectUrl: 'https://myapp.contoso.com'
};

await client.api('/invitations')
    .post(invitation);

```