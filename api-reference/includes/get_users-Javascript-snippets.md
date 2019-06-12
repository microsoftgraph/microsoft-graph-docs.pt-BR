---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d06073d8ecb99b5ad3cd8dd39a48b8c386679c15
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34843525"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{user-id}')
    .get();

```