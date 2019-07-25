---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8dfa0be5e8ddbe891c98fe8b80a3816caf6bd9df
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713063"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/subscriptions/socketIo')
    .version('beta')
    .get();

```