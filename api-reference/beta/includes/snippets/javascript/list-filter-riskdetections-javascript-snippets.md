---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 108fee2b99ddab422a345dd96cbf411aab183372
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46570166"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityProtection/riskDetections')
    .version('beta')
    .filter('riskEventType eq 'unfamiliarFeatures' or riskLevel eq 'medium'')
    .get();

```