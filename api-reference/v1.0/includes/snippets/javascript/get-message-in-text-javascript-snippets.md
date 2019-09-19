---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ce3bd71f9278315fc10f896722fecfc5c2d33ff3
ms.sourcegitcommit: 997fbfe36b518e0a8c230ae2e62666bb5c829e7e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/19/2019
ms.locfileid: "37041938"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/AAMkAGI1AAAoZCfHAAA=/')
    .header('Prefer','outlook.body-content-type="text"')
    .select('subject,body,bodyPreview,uniqueBody')
    .get();

```