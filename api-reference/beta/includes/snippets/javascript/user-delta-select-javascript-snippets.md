---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 24952b8d9451e3c6957f2d6b3fcb2845ffc5954b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716685"
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