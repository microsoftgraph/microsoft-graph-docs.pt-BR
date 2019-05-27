---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e8507936454ad13a21c302b1f0700386b4a526eb
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34481237"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/subscriptions')
    .get();

```