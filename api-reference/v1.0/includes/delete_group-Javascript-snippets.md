---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7c1b6c3997b4e2ac4f39d58f11f958fd99369632
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459014"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}')
    .delete();

```