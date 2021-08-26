---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b7a1c1cee97bd1f11f33499dff6379bb6d6dc4f1f85575e8a6b1618a639425ed
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157250"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/devices/{id}/registeredOwners/{id}/$ref')
    .version('beta')
    .delete();

```