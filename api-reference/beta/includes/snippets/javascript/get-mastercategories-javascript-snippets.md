---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 10469783cfb156c2bd21eaf80194b07ed0780a5c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608261"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/outlook/masterCategories')
    .version('beta')
    .get();

```