---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2aaa1aabc060a947a5a805dc6505f800161ed5ed
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613987"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/pages/{page-id}')
    .version('beta')
    .get();

```