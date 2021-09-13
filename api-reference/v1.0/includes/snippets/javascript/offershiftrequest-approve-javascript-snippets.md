---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 59c69bd79e7fdf27249af5da67db4120343d2875c196cf86ccda85c6add22133
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56900108"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const approve = {
  message: 'Approved!'
};

await client.api('/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/approve')
    .post(approve);

```