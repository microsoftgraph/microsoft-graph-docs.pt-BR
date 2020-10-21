---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0b29eb1ac9c1b85785e96725b0bc7e175e6f8337
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48603766"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/subscribeByMail')
    .post();

```