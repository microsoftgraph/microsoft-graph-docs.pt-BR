---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c6a0fc91fa0adbd4aec8036990ca96a1ae3d9670
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34448024"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/inferenceClassification/overrides')
    .version('beta')
    .get();

```