---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7904e55ab8ed705779a0eb6378293e2f1f8c72b4
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50465161"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/appCatalogs/teamsApps')
    .filter('id eq \'b1c5353a-7aca-41b3-830f-27d5218fe0e5\'')
    .get();

```