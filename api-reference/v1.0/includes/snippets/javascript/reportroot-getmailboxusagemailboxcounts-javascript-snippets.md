---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a0d18136d8f3b6aa6828cc4f72fcf3a8997612db
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733812"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getMailboxUsageMailboxCounts(period='D7')')
    .get();

```