---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cc7baca659dd66b23750c86d4a31559a0bd2b45a
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473946"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let callRecord = await client.api('/communications/callRecords/{id}')
    .get();

```