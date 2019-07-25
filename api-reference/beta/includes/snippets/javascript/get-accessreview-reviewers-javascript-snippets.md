---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 75523fa2ee8308663023fcb03f2b97ae3bfb6d0f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710810"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers')
    .version('beta')
    .get();

```