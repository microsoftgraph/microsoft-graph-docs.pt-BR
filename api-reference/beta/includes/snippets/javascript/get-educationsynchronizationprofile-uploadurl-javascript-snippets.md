---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aa5b6050018a44a65f06f1bb85b8997963e5691e
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48621226"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/synchronizationProfiles/{id}/uploadUrl')
    .version('beta')
    .get();

```