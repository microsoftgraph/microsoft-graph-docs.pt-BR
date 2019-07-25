---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7147fd71f9a33c55f910e3f446d279f860db06a9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35719461"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365ActivationCounts')
    .version('beta')
    .get();

```