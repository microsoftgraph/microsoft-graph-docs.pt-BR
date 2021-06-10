---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2bd07f6e959ee4577f57fde1ee7a84bd12ff273b
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869832"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const timeCard = {
    atAprovedLocation: true,
    notes: {
        contentType: 'text',
        content: 'clock out smaple notes'
    }
};

await client.api('/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972/clockout')
    .version('beta')
    .post(timeCard);

```