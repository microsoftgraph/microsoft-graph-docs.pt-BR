---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d1681b9e265fe845f9bef636d9507fd44aec663b
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997266"
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

let res = await client.api('/me/profile/anniversaries/{id}')
    .version('beta')
    .update(personAnniversary);

```