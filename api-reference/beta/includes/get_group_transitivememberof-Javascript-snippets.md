---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5389e376782c1934937e3e383772dafaee48c33d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34470967"
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