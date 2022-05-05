---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b3462999f58848d3c018eee7addd4f25715efee1
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203605"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let simulationAutomations = await client.api('/security/attackSimulation/simulationAutomations')
    .version('beta')
    .get();

```