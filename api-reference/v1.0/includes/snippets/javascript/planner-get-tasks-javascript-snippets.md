---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 845b69579d22b93ab422e5d0e1c3db8d6a1cfd2f
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/15/2019
ms.locfileid: "37637945"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/tasks')
    .get();

```