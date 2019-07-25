---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ec3369f82fe89f9b3ee2eb92583c903d0ae5ceb4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722290"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getYammerDeviceUsageUserDetail(period='D7')')
    .get();

```