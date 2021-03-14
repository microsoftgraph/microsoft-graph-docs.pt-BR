---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b5519f9c13c12f93841831abf234f8bc24e86b4d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796663"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  displayName: 'Dion Matheson',
  givenName: 'Dion',
  middleName: null,
  surname: 'Matheson',
  mail: 'DionM@contoso.com',
  mobilePhone: '+1 (253) 555-0101',
  createdBy: {
    user: {
      displayName: 'Susana Rocha',
      id: '14012'
    }
  },
  externalSource: 'sis',
  mailingAddress: {
    city: 'Los Angeles',
    countryOrRegion: 'United States',
    postalCode: '98055',
    state: 'CA',
    street: '12345 Main St.'
  },
  primaryRole: 'student',
  residenceAddress: {
    city: 'Los Angeles',
    countryOrRegion: 'United States',
    postalCode: '98055',
    state: 'CA',
    street: '12345 Main St.'
  }
};

await client.api('/education/users')
    .post(educationUser);

```