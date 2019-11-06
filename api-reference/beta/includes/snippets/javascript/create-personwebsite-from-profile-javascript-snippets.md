---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4d21cfa375a2ca499485698bd06023c6f763df6c
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997728"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personWebsite = {
  categories: [
    "categories-value"
  ],
  description: "description-value",
  displayName: "displayName-value",
  webUrl: "webUrl-value"
};

let res = await client.api('/me/profile/websites')
    .version('beta')
    .post(personWebsite);

```