---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b462aa834864261b45480f5326b35954d6844e26
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114030"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let customQuestions = await client.api('/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/customQuestions')
    .version('beta')
    .get();

```