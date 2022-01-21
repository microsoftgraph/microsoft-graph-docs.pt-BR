---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e74a0093289173d9c6d92eedfe1f9eaa3ae6601d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62124189"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const baseTask = {
  destinationTaskListId: 'AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFsPFj7gQqFxG'
};

await client.api('/me/tasks/lists/AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFsPFj7gQpLAt/tasks/AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AkOO4xOT/move')
    .version('beta')
    .post(baseTask);

```