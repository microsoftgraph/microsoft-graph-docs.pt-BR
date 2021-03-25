---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 87e640061bf572f18c43d68145a6223d31e2fbc7
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200895"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  relatedContacts: [
    {
      displayName: 'Father Time',
      emailAddress: 'father@time.com',
      mobilePhone: '4251231234',
      relationship: 'guardian',
      accessConsent: true
    },
    {
      displayName: 'Mother Nature',
      emailAddress: 'mother@nature.co.uk',
      mobilePhone: '3251231234',
      relationship: 'parent',
      accessConsent: true
    }
  ]
};

await client.api('/education/users/{educationUserId}')
    .version('beta')
    .update(educationUser);

```