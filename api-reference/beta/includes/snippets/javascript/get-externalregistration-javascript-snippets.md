---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d8d76cd63dde27559040a4c6038e42bd04592695
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106089"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let meetingRegistration = await client.api('/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration')
    .version('beta')
    .get();

```