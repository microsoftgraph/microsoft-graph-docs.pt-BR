---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0d95adb8a8393d64d897ccb8018c1fe139d4caf9ef07f2bf44fb665568bf333d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329340"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/profile/projects/{id}')
    .version('beta')
    .delete();

```