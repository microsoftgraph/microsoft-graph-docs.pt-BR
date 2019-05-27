---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: de0889463eaf7183573ac40e2e237b9aa65fe5fa
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34446813"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/rejectedSenders')
    .version('beta')
    .get();

```