---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: be69abbca73108410a73a59cb0902347c3285be9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801927"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let driveItem = await client.api('/me/drive/special/{name}')
    .version('beta')
    .get();

```