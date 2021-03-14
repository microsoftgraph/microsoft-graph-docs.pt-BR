---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c2eb4e4f0ac28b5ee9577eb8e3f89be264698092
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790624"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/directory/administrativeUnits/{id}/scopedRoleMembers/{id}')
    .delete();

```