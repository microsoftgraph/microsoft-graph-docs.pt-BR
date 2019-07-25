---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0a273d9e16fbfecd2c73997ced3c505684539a91
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710663"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/administrativeUnits')
    .version('beta')
    .get();

```