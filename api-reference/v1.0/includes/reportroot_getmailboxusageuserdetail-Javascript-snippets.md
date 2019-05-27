---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 269aac21c2b9eca0f425e49ec780d0b7ca88a44d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463358"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getMailboxUsageDetail(period='D7')')
    .get();

```