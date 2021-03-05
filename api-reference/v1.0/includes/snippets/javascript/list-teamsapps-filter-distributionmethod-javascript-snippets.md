---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 245c81829527316a5f0543be6857ea7644b5f3c2
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50465134"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/appCatalogs/teamsApps')
    .filter('distributionMethod eq \'organization\'')
    .get();

```