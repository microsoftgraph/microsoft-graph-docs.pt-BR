---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3db31f97ed1d7e2c04a0a40e79326e643fcef0c6
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34454906"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root')
    .get();

```