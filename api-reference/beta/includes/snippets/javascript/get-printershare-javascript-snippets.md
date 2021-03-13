---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c400e5557068d77820e0349c3be5f1fbbe02cbba
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782339"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printerShare = await client.api('/print/shares/{id}')
    .version('beta')
    .get();

```