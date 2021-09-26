---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eaefdd7dea698893273d948cf1ae53f178e7fb5df645c7e1bddc2e286be60a6b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101603"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let transitiveMemberOf = await client.api('/groups/{id}/transitiveMemberOf')
    .version('beta')
    .get();

```