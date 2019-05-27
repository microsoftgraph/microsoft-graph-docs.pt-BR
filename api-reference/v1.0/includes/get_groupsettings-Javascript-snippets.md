---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b389c27441502a3377ff5d26d343f39b0e49d838
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463167"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groupSettings')
    .get();

```