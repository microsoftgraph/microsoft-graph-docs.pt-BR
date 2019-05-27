---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 20d00a3a409947eb09400d19160a3f37bd62a851
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34472662"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/me/classes')
    .version('beta')
    .get();

```