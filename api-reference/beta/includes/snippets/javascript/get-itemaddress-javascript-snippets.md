---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 95a92b4ce795dccdcec72e35340feccb49f30981d980ac890075eb6cea3ec8fa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158784"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let itemAddress = await client.api('/me/profile/addresses/{id}')
    .version('beta')
    .get();

```