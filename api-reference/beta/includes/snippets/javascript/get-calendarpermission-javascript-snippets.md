---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d74e23a28361089a762470fd2ebd323f26a314662d69bded148ce70e6882db79
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214229"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let calendarPermission = await client.api('/users/{id}/calendar/calendarPermissions/{id}')
    .version('beta')
    .get();

```