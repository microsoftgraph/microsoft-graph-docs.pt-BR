---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: de886246aa436850cbd99e08289481ccd230edfd
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50465382"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getCredentialUsageSummary(period='D30')')
    .version('beta')
    .filter('feature eq \'registration\'')
    .get();

```