---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 47abdb1a1d426829eb65dbe213f2280ba820e6e9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724129"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/licenseDetails')
    .version('beta')
    .get();

```