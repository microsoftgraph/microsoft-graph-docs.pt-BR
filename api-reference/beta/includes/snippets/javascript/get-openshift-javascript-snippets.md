---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 35585ca95ba1f8b785ebb1af6d7a24c379b38ed6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801030"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let openShifts = await client.api('/teams/{id}/schedule/openShifts')
    .version('beta')
    .get();

```