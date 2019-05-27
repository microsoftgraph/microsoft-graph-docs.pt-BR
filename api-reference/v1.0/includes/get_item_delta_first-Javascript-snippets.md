---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4614987000e77e1607091c3d1c0db105688c737c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34457224"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/delta')
    .get();

```