---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fbae0ccee78561f278f20b91dc9ec08de0a0ffac
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223681"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const administrativeUnit = {
  displayName: "displayName-value",
  description: "description-value",
  visibility: "visibility-value"
};

let res = await client.api('/directory/administrativeUnits/{id}')
    .update(administrativeUnit);

```