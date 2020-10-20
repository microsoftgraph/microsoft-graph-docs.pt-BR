---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1058a230b5951dad2c7473933c17560f5d485626
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607444"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/unsubscribeByMail')
    .version('beta')
    .post();

```