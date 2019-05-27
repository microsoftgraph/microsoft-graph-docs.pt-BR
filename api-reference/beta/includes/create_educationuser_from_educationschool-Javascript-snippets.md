---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 903796230c79bd412100af396bedae71175cd132
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480901"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  @odata.id:"https://graph.microsoft.com/beta/education/users/14008"
};

let res = await client.api('/education/schools/'id'/users/$ref')
    .version('beta')
    .post({educationUser : educationUser});

```