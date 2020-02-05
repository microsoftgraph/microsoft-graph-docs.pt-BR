---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 18c5e5061dd44d483724459d603572090d0ce3c9
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774765"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/AlexW@contoso.OnMicrosoft.com/calendar')
    .version('beta')
    .get();

```