---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dd54707a480ffc5b3c6ce4dfbf933b475d6f5358
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444738"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const String = {
  securityEnabledOnly: false
};

let res = await client.api('/groups/{id}/getMemberObjects')
    .version('beta')
    .post(String);

```