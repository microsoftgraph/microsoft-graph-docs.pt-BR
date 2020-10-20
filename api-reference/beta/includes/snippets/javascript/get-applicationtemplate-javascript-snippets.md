---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee7b8bf37e7556c58e407807802ed5bb0e87cc72
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609268"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/applicationTemplates/{id}')
    .version('beta')
    .get();

```