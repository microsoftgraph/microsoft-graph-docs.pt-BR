---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c31acd02c2be4c4db9f1f5e3f96e7721f490c39a
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "43510594"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/administrativeunits/delta')
    .version('beta')
    .get();

```