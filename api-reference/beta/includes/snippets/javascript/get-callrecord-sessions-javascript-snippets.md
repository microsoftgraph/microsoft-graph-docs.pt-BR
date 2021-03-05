---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3d209e9d87e08b4790ed356fc389a5c34262b2e8
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472582"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sessions = await client.api('/communications/callRecords/{id}/sessions')
    .version('beta')
    .get();

```