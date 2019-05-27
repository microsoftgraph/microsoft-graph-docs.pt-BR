---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 97b7984ee950eb99b206296337f65b7cbaaddadf
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34446488"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/scopedAdministratorOf')
    .version('beta')
    .get();

```