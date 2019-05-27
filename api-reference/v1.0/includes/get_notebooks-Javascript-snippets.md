---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 628ad7fe31632c0ddae3959b1a2101b59bd57ebc
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34477478"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/notebooks')
    .get();

```