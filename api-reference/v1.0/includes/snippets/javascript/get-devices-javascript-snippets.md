---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6609f6fb126712a19c4570bb98e3adede5f85e72
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797980"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let devices = await client.api('/devices')
    .get();

```