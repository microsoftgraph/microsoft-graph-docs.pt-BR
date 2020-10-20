---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 749f7edfebb38b0e3ef34df6aa12b0bfdc8aea7f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48621838"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/programControlTypes')
    .version('beta')
    .get();

```