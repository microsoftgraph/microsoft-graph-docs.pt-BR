---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 819775019f2b43bc5967659d4c49653c6a43e3ae
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728867"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/outlook/supportedTimeZones')
    .version('beta')
    .get();

```