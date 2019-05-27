---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c2b095965cb74b95a2037d872f3ec8743985c2e3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34454871"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityProviders/Amazon-OAuth')
    .get();

```