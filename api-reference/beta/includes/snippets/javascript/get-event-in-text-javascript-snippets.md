---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 06f6a288b6c6ef1e054b324e3dca69219b3ee4c4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801693"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let event = await client.api('/me/events/AAMkAGI1AAAoZDOFAAA=/')
    .version('beta')
    .header('Prefer','outlook.body-content-type="text"')
    .select('subject,body,bodyPreview')
    .get();

```