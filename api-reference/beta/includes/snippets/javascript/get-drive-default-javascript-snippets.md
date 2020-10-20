---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 308c9270f584c97176a4eb6b305a46590eb29f5a
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607925"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive')
    .version('beta')
    .get();

```