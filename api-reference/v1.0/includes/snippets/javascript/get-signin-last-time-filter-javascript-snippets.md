---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c8cef08bd011b73f6d9814a374ae34fe81c7b594
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905678"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users')
    .filter('startswith(displayName,'Eric'),')
    .select('displayName,signInActivity')
    .get();

```