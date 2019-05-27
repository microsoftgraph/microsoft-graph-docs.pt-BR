---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cd369fb3dca0090a68fab8a8eb5ca0dccb7cb818
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34481468"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/security/secureScoreControlProfiles')
    .get();

```