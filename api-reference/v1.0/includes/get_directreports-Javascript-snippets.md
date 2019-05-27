---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0234838742ff96c8e927c235ecdc772a130bde0a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34479753"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/directReports')
    .get();

```