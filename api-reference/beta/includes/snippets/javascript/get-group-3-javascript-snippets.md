---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 43ebeba990955a66630d7689b4a50881b3eb9469
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961327"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let group = await client.api('/termStore/groups/{groupId}')
    .version('beta')
    .get();

```