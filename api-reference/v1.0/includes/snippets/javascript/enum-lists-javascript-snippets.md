---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 06542a543bd1471cd45583317e3d18811629236a
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616158"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/lists')
    .get();

```