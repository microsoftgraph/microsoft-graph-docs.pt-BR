---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ffa3869ba55b36eb0c4d0ed808494d939f229448
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081219"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/delta')
    .version('beta')
    .get();

```