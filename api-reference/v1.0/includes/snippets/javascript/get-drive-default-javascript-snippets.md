---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: acf2af8d025c2f2ada9b6e1ecdff3a3e82e819d9
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48610591"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive')
    .get();

```