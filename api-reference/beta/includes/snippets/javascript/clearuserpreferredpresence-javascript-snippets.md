---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 500ba1bae9bf9b727c435d125337b993a006a587
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61524831"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const clearUserPreferredPresence = {
};

await client.api('/users/fa8bf3dc-eca7-46b7-bad1-db199b62afc3/presence/clearUserPreferredPresence')
    .version('beta')
    .post(clearUserPreferredPresence);

```