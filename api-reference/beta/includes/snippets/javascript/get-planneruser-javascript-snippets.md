---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2c3ea822d5696db839bb9d57eed0303fc542f1bb
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475434"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerUser = await client.api('/me/planner')
    .version('beta')
    .get();

```