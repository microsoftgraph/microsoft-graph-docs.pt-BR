---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a83d9e312e1484148205baf09e0296bfe95ba222
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013463"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users')
    .header('ConsistencyLevel','eventual')
    .filter('endswith(mail,'a@contoso.com'),')
    .orderby('userPrincipalName ')
    .get();

```