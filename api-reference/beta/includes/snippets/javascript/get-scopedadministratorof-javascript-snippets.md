---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 97b7984ee950eb99b206296337f65b7cbaaddadf
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716471"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/scopedAdministratorOf')
    .version('beta')
    .get();

```