---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d36aac046727200bab0c516a21efea7754a17df3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783786"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let driveItem = await client.api('/shares/{shareIdOrUrl}/driveItem')
    .expand('children')
    .get();

```