---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 99f930a1d47b772a340ea6d6c351b1bc1296a789
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792674"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/renew')
    .post();

```