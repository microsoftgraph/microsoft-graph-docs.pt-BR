---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1058a230b5951dad2c7473933c17560f5d485626
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444633"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/unsubscribeByMail')
    .version('beta')
    .post();

```