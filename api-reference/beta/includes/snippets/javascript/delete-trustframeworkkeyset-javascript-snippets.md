---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eab3b2ce5352d5d90f5e1c8906101c98344b9208
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938272"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/trustFramework/keySets/{id}')
    .version('beta')
    .delete();

```