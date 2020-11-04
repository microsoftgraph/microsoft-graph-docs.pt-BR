---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8ebc2ccf95c140147471c1d4593dbd8ce0fc63e1
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903661"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/members/microsoft.graph.user')
    .header('ConsistencyLevel','eventual')
    .search('displayName:Pr')
    .select('displayName,id')
    .orderby('displayName ')
    .get();

```