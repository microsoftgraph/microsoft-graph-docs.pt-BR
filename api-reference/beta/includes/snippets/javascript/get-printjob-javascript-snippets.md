---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0befbe07591023792e49808056a32ed1fdebf717
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784885"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printJob = await client.api('/print/printers/c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb/jobs/5182')
    .version('beta')
    .get();

```