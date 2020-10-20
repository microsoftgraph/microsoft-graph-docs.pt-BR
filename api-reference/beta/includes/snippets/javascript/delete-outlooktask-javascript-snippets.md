---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fb24eaac349928e1e0f6570681c65344ba6ee3c0
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607702"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/outlook/tasks/AAMkADIyAAAhrb_QAAA=')
    .version('beta')
    .delete();

```