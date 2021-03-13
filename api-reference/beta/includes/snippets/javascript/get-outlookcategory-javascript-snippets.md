---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 30f8d69ee192d23fe4cb028e2664c2124747d839
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778649"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let outlookCategory = await client.api('/me/outlook/masterCategories/de912e4d-c790-4da9-949c-ccd933aaa0f7')
    .version('beta')
    .get();

```