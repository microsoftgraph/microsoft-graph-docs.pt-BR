---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8504b8579eaa8c46876e4040d724df9418b06b10
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774776"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/AlexW@contoso.OnMicrosoft.com/mailboxsettings')
    .version('beta')
    .get();

```