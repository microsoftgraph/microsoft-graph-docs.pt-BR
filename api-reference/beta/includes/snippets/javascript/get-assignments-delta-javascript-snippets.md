---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 242ca7c61cdc23a3bb84a518f273d2a087a61708
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137557"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/delta')
    .version('beta')
    .get();

```