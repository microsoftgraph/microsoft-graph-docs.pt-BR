---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3fe7fc1f0d25bdcb147c3b876b2c3584fd2441505706eda8f86263823102f0af
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099663"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let informationProtectionLabel = await client.api('/me/informationprotection/policy/labels/{id}')
    .version('beta')
    .get();

```