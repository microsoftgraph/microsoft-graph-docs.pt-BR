---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 47008784717d4f04b7302dd2a2d058854c409b20458b8e92cd208fa83e6f1b9c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899087"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let privilegedApproval = await client.api('/privilegedApproval/{id}')
    .version('beta')
    .get();

```