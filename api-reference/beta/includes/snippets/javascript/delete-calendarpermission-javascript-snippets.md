---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ab35fb0bf6fb4094339a2ccfd9937666316b2ad28990af5342a040c022c48a44
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214234"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/{id}/calendar/calendarPermissions/{id}')
    .version('beta')
    .delete();

```