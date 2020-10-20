---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f161b07de78b624455a17aaabcad12dae9d24a8d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620215"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/special/{name}')
    .version('beta')
    .get();

```