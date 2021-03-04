---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e19ca488f1af3c453165ee1f0248eade14f7bc3b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440770"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityProtection/riskyUsers')
    .version('beta')
    .filter('riskLevel eq microsoft.graph.riskLevel\'medium\'')
    .get();

```