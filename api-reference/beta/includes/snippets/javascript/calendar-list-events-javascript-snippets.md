---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e2d6fa08bb2c826c79fa4b5abd1ccceac3fe3972
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996082"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let events = await client.api('/me/calendar/events')
    .version('beta')
    .filter('startsWith(subject,\'All\')')
    .get();

```