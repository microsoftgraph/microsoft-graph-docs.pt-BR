---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4f8be3019a6f75014d529e1daf9c4c21a99aa0fa2249d5c8faa9cd44399ef9f0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214646"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/mailFolders/AAMkAGVmMDEzM/')
    .version('beta')
    .delete();

```