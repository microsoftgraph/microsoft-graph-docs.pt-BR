---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f03e4e33462c776323c454be708c02b5d0295a6f
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61524775"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const move = {
  destinationTaskListId: 'AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFsPFj7gQqFxG'
};

await client.api('/me/tasks/lists/AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFsPFj7gQpLAt/tasks/AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AkOO4xOT/move')
    .version('beta')
    .post(move);

```