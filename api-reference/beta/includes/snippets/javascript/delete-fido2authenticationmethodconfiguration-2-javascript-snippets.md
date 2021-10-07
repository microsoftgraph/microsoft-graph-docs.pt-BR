---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 503be85280198f092b422578a8a919e4d65bba01de5323dee175c1a983f968c3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329634"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass')
    .version('beta')
    .delete();

```