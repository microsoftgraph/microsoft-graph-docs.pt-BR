---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f6522b6e897e9d55798349b478bfc08bed3a7051
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34455269"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSharePointActivityPages(period='D7')')
    .get();

```