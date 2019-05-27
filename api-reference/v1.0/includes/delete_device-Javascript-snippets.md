---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 97c255c7140f46aa8f99c1d79a31d461db79b38c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459346"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/devices/{id}')
    .delete();

```