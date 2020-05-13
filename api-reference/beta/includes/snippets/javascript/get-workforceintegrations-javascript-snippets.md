---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a9e655ef561c1ec5e7b99881dc4625e4a165bde3
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "40870575"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teamwork/workforceIntegrations')
    .version('beta')
    .get();

```