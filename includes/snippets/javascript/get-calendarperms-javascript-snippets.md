---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 03687527787ec827b0012dc0f81cfbfef4b3ed08e111b83c0c932cec57dec3fa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237018"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/AlexW@contoso.OnMicrosoft.com/calendar/calendarPermissions')
    .version('beta')
    .get();

```