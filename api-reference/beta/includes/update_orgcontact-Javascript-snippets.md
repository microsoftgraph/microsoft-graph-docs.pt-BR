---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 066ebd0e00f5f6b1f7f5a117ae24fe4b765c6693
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34460689"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const orgContact = {
  businessPhones: [
    "businessPhones-value"
  ],
  city: "city-value",
  companyName: "companyName-value",
  country: "country-value",
  department: "department-value",
  displayName: "displayName-value"
};

let res = await client.api('/contacts/{id}')
    .version('beta')
    .update({orgContact : orgContact});

```