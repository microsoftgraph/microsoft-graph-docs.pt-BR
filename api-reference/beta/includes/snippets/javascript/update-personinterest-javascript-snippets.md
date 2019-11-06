---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f5e4e42b18e17a82548751aad9b8c19f3d1592ee
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998097"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personInterest = {
  categories: [
    "categories-value"
  ],
  description: "description-value",
  displayName: "displayName-value",
  webUrl: "webUrl-value"
};

let res = await client.api('/me/profile/interests/{id}')
    .version('beta')
    .update(personInterest);

```