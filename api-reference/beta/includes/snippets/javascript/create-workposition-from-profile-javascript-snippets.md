---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 71a63456ab9101bcb67153f017890ff75ebdea0f
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820334"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workPosition = {
  detail: {
    company: {
      displayName: "Adventureworks Ltd.",
      department: "Consulting",
      officeLocation: "AW23/344",
      address: {
        type: "business",
        street: "123 Patriachy Ponds",
        city: "Moscow",
        countryOrRegion: "Russian Federation",
        postalCode: "RU-34621"
      },
      webUrl: "https://www.adventureworks.com"
    },
    jobTitle: "Senior Product Branding Manager II",
    role: "consulting",
  },
  isCurrent: true
};

let res = await client.api('/me/profile/positions')
    .version('beta')
    .post(workPosition);

```