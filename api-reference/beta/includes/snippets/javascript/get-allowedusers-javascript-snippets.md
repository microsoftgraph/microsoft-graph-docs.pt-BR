---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 00c8d19e819b90aff695d10e137584dc7b2b2550
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44216816"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/shares/{id}/allowedUsers')
    .version('beta')
    .get();

```