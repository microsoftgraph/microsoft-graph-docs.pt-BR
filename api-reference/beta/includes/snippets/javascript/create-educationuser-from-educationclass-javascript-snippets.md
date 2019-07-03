---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9638b89d82e1da4386e12a01f36164a570f13385
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519233"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  @odata.id:"https://graph.microsoft.com/beta/education/users/14011"
};

let res = await client.api('/education/classes/11017/teachers/$ref')
    .version('beta')
    .post({educationUser : educationUser});

```