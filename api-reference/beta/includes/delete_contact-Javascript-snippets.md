---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: db911671d1b74faf586141c5743c0cb909099609
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34438711"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/contacts/{id}')
    .version('beta')
    .delete();

```