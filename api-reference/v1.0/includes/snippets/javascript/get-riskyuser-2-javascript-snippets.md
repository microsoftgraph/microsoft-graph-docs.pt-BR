---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3fb0d548e5c9207eb3f927f0b2fc256b2c406f26
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62134349"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let riskyUsers = await client.api('/identityProtection/riskyUsers')
    .get();

```