---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 268d52a604c904c8970f3fa9bcfafe7fc5bbf051
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604154"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/revokeSignInSessions')
    .version('beta')
    .post();

```