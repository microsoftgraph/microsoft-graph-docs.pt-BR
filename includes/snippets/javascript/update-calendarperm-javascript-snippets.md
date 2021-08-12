---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 214e19d2cb41b0edbdab1bd485633f1bd3e02ca2fd1bc3b5238a3d90fe035a9a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237022"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendarPermission = {
  role: "write"
};

let res = await client.api('/users/AlexW@contoso.OnMicrosoft.com/calendars/AAMkADAwAABf02bAAAA=/calendarPermissions/L289RXhjaGFuZ2VMYWJQWRlbGVW')
    .version('beta')
    .update(calendarPermission);

```