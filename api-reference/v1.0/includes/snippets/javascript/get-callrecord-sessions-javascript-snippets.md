---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 64092b874e110de29838e1a0d50494d9c14f5cc5
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473879"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sessions = await client.api('/communications/callRecords/{id}/sessions')
    .get();

```