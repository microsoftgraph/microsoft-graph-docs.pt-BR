---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 73c3c3f14c503c767621bd9078497f8d6e50b515d49d2e32be9de2aa989c0900
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156247"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let b2xUserFlows = await client.api('/identity/b2xUserFlows')
    .version('beta')
    .get();

```