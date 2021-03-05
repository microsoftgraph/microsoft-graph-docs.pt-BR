---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 54ba2c4e4fb91047be13043bda84ca925547ff67
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472592"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let callRecord = await client.api('/communications/callRecords/{id}')
    .version('beta')
    .get();

```