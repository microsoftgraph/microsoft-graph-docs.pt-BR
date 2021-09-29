---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 84dd6f2621679f973752c467037acb0964121cb6
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996204"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendarPermission = {
    emailAddress: {
        name: 'Samantha Booth',
        address: 'samanthab@adatum.onmicrosoft.com'
    },
    isInsideOrganization: true,
    isRemovable: true,
    role: 'read'
};

await client.api('/me/calendar/calendarPermissions')
    .post(calendarPermission);

```