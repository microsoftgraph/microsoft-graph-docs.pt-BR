---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 23e250ee4e79d391d060c18965440c9fa24fd79a
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996065"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workPosition = {
  categories: [
    "categories-value"
  ],
  detail: {
    company: {
      displayName: "displayName-value",
      pronunciation: "pronunciation-value",
      department: "department-value",
      officeLocation: "officeLocation-value",
      address: {
        type: "type-value",
        postOfficeBox: "postOfficeBox-value",
        street: "street-value",
        city: "city-value",
        state: "state-value",
        countryOrRegion: "countryOrRegion-value",
        postalCode: "postalCode-value"
      },
      webUrl: "webUrl-value"
    },
    description: "description-value",
    endMonthYear: "datetime-value",
    jobTitle: "jobTitle-value",
    role: "role-value",
    startMonthYear: "datetime-value",
    summary: "summary-value"
  }
};

let res = await client.api('/me/profile/positions/{id}')
    .version('beta')
    .update(workPosition);

```