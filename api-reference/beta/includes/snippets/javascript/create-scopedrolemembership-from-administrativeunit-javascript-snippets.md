---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6c6223d7b63fe2e4d03290ceab9a8793e461c123
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808108"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const scopedRoleMembership = {
  roleId: 'roleId-value',
  roleMemberInfo: {
    id: 'id-value'
  }
};

await client.api('/administrativeUnits/{id}/scopedRoleMembers')
    .version('beta')
    .post(scopedRoleMembership);

```