---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8141bebcf8ef89c3a33cb6aa5026ede1844fe2fa
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34441490"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365GroupsActivityDetail(period='D7')')
    .version('beta')
    .get();

```