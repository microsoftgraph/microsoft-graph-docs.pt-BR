---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1ec8cc9640301fd3956b28b81650271bc843b7ef4905e0f99fa974e88b96b8e6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101834"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cancel = {
  cancellationMessage: 'Your appointment has been successfully cancelled. Please call us again.'
};

await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKoAAA=/cancel')
    .version('beta')
    .post(cancel);

```