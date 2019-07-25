---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 343047d66f1871d52e18068a4970b5791a6a28bf
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722372"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getYammerActivityUserDetail(period='D7')')
    .get();

```