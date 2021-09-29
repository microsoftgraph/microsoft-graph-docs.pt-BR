---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2bd0d9f4377ec08e2161dcd770344d45db4cb5ea
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2021
ms.locfileid: "59997026"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/organization/84841066-274d-4ec0-a5c1-276be684bdd3/branding')
    .version('beta')
    .delete();

```