---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c8d4b59c27508440e59caeef606ad59c5c2fc396
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50465142"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/appCatalogs/teamsApps')
    .version('beta')
    .filter('distributionMethod eq \'organization\'')
    .get();

```