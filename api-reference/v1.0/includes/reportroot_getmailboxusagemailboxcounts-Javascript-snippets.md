---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a0d18136d8f3b6aa6828cc4f72fcf3a8997612db
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34465075"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getMailboxUsageMailboxCounts(period='D7')')
    .get();

```