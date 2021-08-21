---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e783b13ed5751917440a58f4228fa8085eaf1cbdd4f413604fe894b2010e5261
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213740"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let assignments = await client.api('/privilegedRoles/{id}/assignments')
    .version('beta')
    .get();

```