---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 454f962d528d78da0bd886fcbda879896d332993
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612440"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/{id}/createForward')
    .post();

```