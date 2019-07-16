---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 73d3f6f34a91250558f4d13e3a323198a7a46b15
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740764"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendar = {
  name: "Social events"
};

let res = await client.api('/me/calendar')
    .update({calendar : calendar});

```