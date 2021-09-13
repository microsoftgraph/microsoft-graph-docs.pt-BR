---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b8b670644d2ba58322f2e29419539887a6d98a5f7213b64981df7ab465cf7f01
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272805"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/{id}/calendar/calendarPermissions/{id}')
    .delete();

```