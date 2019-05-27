---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f155d22ffbb26993694d34b9d786e2251730a190
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459218"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/events/{id}')
    .delete();

```