---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: af9f06e290f9581e64e3ee4262f6c55839ef6e3a88ebdbd7e73fc20e95e34d98
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273387"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let windowsHelloForBusinessMethods = await client.api('/users/annie@contoso.com/authentication/windowsHelloForBusinessMethods')
    .version('beta')
    .get();

```