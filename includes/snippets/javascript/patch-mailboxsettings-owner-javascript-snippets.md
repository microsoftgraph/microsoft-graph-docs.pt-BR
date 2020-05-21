---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b8bd9075882b69002a3a94aa4bfd9c3b05017564
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774779"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailboxSettings = {
  delegateMeetingMessageDeliveryOptions: "sendToDelegateAndPrincipal"
};

let res = await client.api('/users/AlexW@contoso.OnMicrosoft.com/mailboxsettings')
    .version('beta')
    .update(mailboxSettings);

```