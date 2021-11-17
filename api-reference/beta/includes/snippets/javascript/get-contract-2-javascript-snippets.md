---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 92f347083c31bc0fec5c39b033ba44d44b24a7dd25e424b1b676c4b2e71caeaa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56897943"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contracts = await client.api('/contracts')
    .version('beta')
    .get();

```