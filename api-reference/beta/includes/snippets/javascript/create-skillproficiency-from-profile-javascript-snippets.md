---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 997ad7532dbd1041d4628feb0c47b24911a52e43
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821103"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const skillProficiency = {
  categories: [
    "Professional"
  ],
  allowedAudiences: "organization",
  displayName: "API Design",
  proficiency: "generalProfessional",
  collaborationTags: [
    "ableToMentor"
  ]
};

let res = await client.api('/me/profile/skills')
    .version('beta')
    .post(skillProficiency);

```