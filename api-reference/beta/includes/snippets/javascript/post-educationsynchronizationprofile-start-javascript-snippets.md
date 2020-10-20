---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1eceaeeb8212ee05cbb8c73b046820cf37cc8f38
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605630"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/synchronizationProfiles/{id}/start')
    .version('beta')
    .post();

```