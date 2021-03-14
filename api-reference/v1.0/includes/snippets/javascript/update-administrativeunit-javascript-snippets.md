---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 26b16a309baa8f65e1b088f5997e3556fbeb43e0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800810"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const administrativeUnit = {
  displayName: 'displayName-value',
  description: 'description-value',
  visibility: 'visibility-value'
};

await client.api('/directory/administrativeUnits/{id}')
    .update(administrativeUnit);

```