---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 71043814d9b930ebc10679fd7c0d0ebc71c203cc
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721687"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/AAMkAGVmMDEzM')
    .version('beta')
    .get();

```