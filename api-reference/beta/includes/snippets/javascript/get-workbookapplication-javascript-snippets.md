---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cbd798532a7288116e6d71121087d23db33e2cd7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809540"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookApplication = await client.api('/me/drive/items/{id}/workbook/application')
    .version('beta')
    .get();

```