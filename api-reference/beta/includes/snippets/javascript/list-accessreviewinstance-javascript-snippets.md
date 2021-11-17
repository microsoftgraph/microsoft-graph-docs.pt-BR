---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a72692ebafc8aa70d3160dcb57c10816786964a42a6e9782e073f2c572c08018
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898194"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let instances = await client.api('/identityGovernance/accessReviews/definitions/8564a649-4f67-4e09-88e7-55def6530e88/instances')
    .version('beta')
    .skip(0)
    .top(100)
    .get();

```