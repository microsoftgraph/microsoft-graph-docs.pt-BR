---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 44fa434585498096699c2011d1129f9ec3991676
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34451661"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityProviders')
    .get();

```