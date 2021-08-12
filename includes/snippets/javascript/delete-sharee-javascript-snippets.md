---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8254b85f6b4d9b6dfb8c21c75786b2c9468dd921422fc6654a816884da4981bb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237019"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/AlexW@contoso.OnMicrosoft.com/calendars/AAMkADAwAABf02bAAAA=/calendarPermissions/L289RXhjaGFuZ2VMYWJTWVnYW5C')
    .version('beta')
    .delete();

```