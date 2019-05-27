---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c18fc8c4751b1476eb5fc17e38fd71b31a751aad
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34450437"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/delta')
    .version('beta')
    .header('Prefer','return=minimal')
    .select('displayName,jobTitle,mobilePhone')
    .get();

```