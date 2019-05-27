---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e20f47df29c1574c8389ea36457efb0981d59254
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34456844"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/channels/{id}')
    .get();

```