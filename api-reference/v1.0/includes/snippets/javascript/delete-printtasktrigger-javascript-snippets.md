---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d7401aa68f0b7900494a66a8594a7fc69f435827
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772020"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/printers/{printerId}/taskTriggers/{printTaskTriggerId}')
    .delete();

```