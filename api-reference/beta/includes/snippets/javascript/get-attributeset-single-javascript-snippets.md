---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 25aed7cbb9f1bf15fc3785c8bcd04a9805c52312
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61223615"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let attributeSet = await client.api('/directory/attributeSets/Engineering')
    .version('beta')
    .get();

```