---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ce6da6532711f7164f3b5fa701deca93ff6db604748a3e66ac5e093ffec019f6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215182"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/drives/{drive-id}/items/{item-id}/checkout')
    .version('beta')
    .post();

```