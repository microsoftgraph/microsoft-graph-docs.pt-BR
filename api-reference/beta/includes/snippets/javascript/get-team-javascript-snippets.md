---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: defc31e78b6a81327ef820b576c7ef502f71aca9
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332468"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}')
    .version('beta')
    .get();

```