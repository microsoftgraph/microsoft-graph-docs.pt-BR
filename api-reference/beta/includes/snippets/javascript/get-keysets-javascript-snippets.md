---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d0c4a4c24ee5a290b95348891ec1a0989e31da7e
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938330"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/trustFramework/keySets')
    .version('beta')
    .get();

```