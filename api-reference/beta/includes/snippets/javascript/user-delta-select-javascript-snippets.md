---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 24952b8d9451e3c6957f2d6b3fcb2845ffc5954b
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615799"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/delta')
    .version('beta')
    .select('displayName,jobTitle,mobilePhone')
    .get();

```