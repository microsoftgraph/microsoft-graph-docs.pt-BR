---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 41bd109af277a6dcbecc4e0ef5c978f3c75d7d522d4b6010a9f32733d221518c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57160306"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tasks = await client.api('/me/outlook/tasks')
    .version('beta')
    .get();

```