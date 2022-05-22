---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1e16f97c1b35fa93dcabf6c331b4d32414e5698c
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629435"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/delta')
    .get();

```