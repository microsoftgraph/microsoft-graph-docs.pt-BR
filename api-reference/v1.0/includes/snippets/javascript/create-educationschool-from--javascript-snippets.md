---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ea5cef8b89bdd786fbc118b2d858ccc5dec128b8
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474811"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationSchool = {
  '@odata.type': '#microsoft.graph.educationSchool',
  displayName: 'String',
  description: 'String',
  externalSource: 'String',
  externalSourceDetail: 'String',
  principalEmail: 'String',
  principalName: 'String',
  externalPrincipalId: 'String',
  lowestGrade: 'String',
  highestGrade: 'String',
  schoolNumber: 'String',
  externalId: 'String',
  phone: 'String',
  fax: 'String',
  createdBy: {
    '@odata.type': 'microsoft.graph.identitySet'
  },
  address: {
    '@odata.type': 'microsoft.graph.physicalAddress'
  }
};

await client.api('/education/schools')
    .post(educationSchool);

```