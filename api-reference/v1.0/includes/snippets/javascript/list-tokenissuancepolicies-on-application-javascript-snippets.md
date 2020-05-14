---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b82030fe3c35bb29b08af5ec8d65daae50807d9e
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "43510515"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/applications/{id}/tokenIssuancePolicies')
    .get();

```