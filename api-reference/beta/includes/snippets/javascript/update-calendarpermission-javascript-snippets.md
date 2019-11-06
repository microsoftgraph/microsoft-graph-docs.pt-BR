---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 835accaa80091ea19293b05e8ac221cf55f962c9
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994832"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendarPermission = {
  emailAddress: {
    name: "My Organization",
  },
  isRemovable: true,
  isInsideOrganization: true,
  role: "write",
  allowedRoles: [
    "none",
    "freeBusyRead",
    "limitedRead",
    "read",
    "write"
  ],
  id: "RGVmYXVsdA=="
};

let res = await client.api('/users/{id}/calendar/calendarPermissions/{id}')
    .version('beta')
    .update(calendarPermission);

```