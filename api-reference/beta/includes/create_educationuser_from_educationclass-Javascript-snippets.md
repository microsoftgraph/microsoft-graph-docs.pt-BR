---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9638b89d82e1da4386e12a01f36164a570f13385
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480943"
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