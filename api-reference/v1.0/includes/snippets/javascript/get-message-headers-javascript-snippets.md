---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d8bd2f45de0b5ad816a5d459eee327b52d39e450
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604156"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/AAMkADhAAAW-VPeAAA=/')
    .select('internetMessageHeaders')
    .get();

```