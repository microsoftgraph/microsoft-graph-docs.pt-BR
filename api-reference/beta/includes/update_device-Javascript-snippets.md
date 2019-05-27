---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 324d0ba94693ad9c39cab2e20b63baf30950ed5f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34461324"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const device = {
  accountEnabled: false
};

let res = await client.api('/devices/{id}')
    .version('beta')
    .update({device : device});

```