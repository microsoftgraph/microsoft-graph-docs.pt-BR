---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 64b7670e4d32322d0e486185cc8e840dc56462c0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34440342"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/recent')
    .get();

```