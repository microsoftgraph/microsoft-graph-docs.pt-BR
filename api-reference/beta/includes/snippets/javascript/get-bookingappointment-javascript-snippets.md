---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a6d1c27a09154eb79dba4196615f086992c4371c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094801"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bookingAppointment = await client.api('/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/appointments/AAMkADKnAAA=')
    .version('beta')
    .get();

```