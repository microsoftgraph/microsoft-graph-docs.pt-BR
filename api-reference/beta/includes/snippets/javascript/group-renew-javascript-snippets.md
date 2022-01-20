---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7908bab7f9e16cb46cf4b8053fe6b53d8604e603
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113333"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/renew')
    .version('beta')
    .post();

```