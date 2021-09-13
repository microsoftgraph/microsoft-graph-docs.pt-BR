---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dff8141d6cd1e92e45b57f09e33edf3fa730d80a2fbffe4181f71df8c26727d9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213975"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personCertification = {
  issuingAuthority: 'International Academy of Marketing Excellence',
  issuingCompany: 'International Academy of Marketing Excellence'
};

await client.api('/users/{userId}/profile/certifications/{id}')
    .version('beta')
    .update(personCertification);

```