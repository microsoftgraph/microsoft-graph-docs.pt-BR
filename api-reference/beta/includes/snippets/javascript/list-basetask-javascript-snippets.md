---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 34179513b7de9e6c84f96dec61a70d2fd181b7aa
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525447"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tasks = await client.api('/me/tasks/lists/AQMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNm/tasks')
    .version('beta')
    .get();

```