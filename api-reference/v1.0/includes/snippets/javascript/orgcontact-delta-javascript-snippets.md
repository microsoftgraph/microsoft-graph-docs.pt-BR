---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b1dfd2c1ba03525de2a57dfd1931285ca8e421a226e8fba170f311677b13e152
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214337"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/contacts/delta')
    .get();

```