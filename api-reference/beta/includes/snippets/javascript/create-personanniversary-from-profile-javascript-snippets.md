---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c3376a86f41a117440444d67de1b6c14065e5af9
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "37996578"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personAnniversary = {
  type: "type-value",
  date: "datetime-value"
};

let res = await client.api('/me/profile/anniversaries')
    .version('beta')
    .post(personAnniversary);

```