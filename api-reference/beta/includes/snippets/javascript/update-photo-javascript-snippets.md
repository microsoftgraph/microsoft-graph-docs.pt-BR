---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8322c3da19c7c81745947ef69e03ae2ebe38dce9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35498452"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const profilePhoto = {
  height: 99,
  width: 99,
  id: "id-value"
};

let res = await client.api('/users/{id|userPrincipalName}/photo')
    .version('beta')
    .update({profilePhoto : profilePhoto});

```