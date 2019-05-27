---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c27b814f3058564eb0cbb05f819e6d2c26cdf4df
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34482266"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/unsubscribeByMail')
    .post();

```