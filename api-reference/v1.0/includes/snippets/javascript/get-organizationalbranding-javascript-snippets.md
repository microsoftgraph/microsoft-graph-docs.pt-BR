---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e559eb230267e3e855ef478e149ed5b20ab93885
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2021
ms.locfileid: "59997067"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let organizationalBranding = await client.api('/organization/84841066-274d-4ec0-a5c1-276be684bdd3/branding')
    .get();

```