---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: db509a71db03f8a6ed7f76fb010132bb683f8c86fd41d2baae4415cc114dc237
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159649"
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