---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d7f8334d453fb0e0b17e18dd6feafa2bf6196a051f0fd12eda653e62c92941a5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899060"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let riskyUsers = await client.api('/identityProtection/riskyUsers')
    .version('beta')
    .get();

```