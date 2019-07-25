---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 76646b569e9c45480d0ac67ff5e62f5c2c9c48f3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729885"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/delta')
    .version('beta')
    .get();

```