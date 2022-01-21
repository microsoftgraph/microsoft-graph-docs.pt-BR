---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e88986d90e38144900ac5cd6edd84a59900a59d0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094836"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const bookingAppointment = {
    '@odata.type':'#microsoft.graph.bookingAppointment',
    end: {
        '@odata.type':'#microsoft.graph.dateTimeTimeZone',
        dateTime: '2018-05-06T12:30:00.0000000+00:00',
        timeZone: 'UTC'
    },
    invoiceDate: {
        '@odata.type':'#microsoft.graph.dateTimeTimeZone',
        dateTime: '2018-05-06T12:30:00.0000000+00:00',
        timeZone: 'UTC'
    },
    start: {
        '@odata.type':'#microsoft.graph.dateTimeTimeZone',
        dateTime: '2018-05-06T12:00:00.0000000+00:00',
        timeZone: 'UTC'
    }
};

await client.api('/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/appointments/AAMkADKnAAA=')
    .version('beta')
    .update(bookingAppointment);

```