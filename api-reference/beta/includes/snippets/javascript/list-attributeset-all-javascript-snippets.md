---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ea236888cc66b80af48b84ead1d894b641662d33
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61225514"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let attributeSets = await client.api('/directory/attributeSets')
    .version('beta')
    .get();

```