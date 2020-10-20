---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5389e376782c1934937e3e383772dafaee48c33d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620393"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/transitiveMemberOf')
    .version('beta')
    .get();

```