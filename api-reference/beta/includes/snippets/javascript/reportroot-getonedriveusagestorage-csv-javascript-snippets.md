---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 54ba0d5865ed42cc38d01d75e3b695a6f71ce0af
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35727129"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOneDriveUsageStorage(period='D7')')
    .version('beta')
    .get();

```