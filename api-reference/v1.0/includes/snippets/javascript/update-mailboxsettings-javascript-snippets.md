---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c5dac2f0f70fc7246b1761e01459b53091d4e5af
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35465893"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailboxSettings = {
    @odata.context: "https://graph.microsoft.com/v1.0/$metadata#Me/mailboxSettings",
    automaticRepliesSetting: {
        status: "Scheduled",
        scheduledStartDateTime: {
          dateTime: "2016-03-20T18:00:00.0000000",
          timeZone: "UTC"
        },
        scheduledEndDateTime: {
          dateTime: "2016-03-28T18:00:00.0000000",
          timeZone: "UTC"
        }
    }
};

let res = await client.api('/me/mailboxSettings')
    .update({mailboxSettings : mailboxSettings});

```