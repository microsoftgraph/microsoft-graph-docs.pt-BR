---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 631b66ef72c9618d381e18cb96f761c9d2eaf541
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620876"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/AAMkAGVmMDEz/')
    .version('beta')
    .select('internetMessageHeaders')
    .get();

```