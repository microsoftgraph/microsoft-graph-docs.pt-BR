---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7539c3e65f318cd8e3fe79c87288c6e16444ccc0fe2d72e78bb76026cf4aaf87
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101848"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let recoveryKeys = await client.api('/informationProtection/bitlocker/recoveryKeys')
    .version('beta')
    .header('ocp-client-name','"My Friendly Client"')
    .header('ocp-client-version','"1.2"')
    .get();

```