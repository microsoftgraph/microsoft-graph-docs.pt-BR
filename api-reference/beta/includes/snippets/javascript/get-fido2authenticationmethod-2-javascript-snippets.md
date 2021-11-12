---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d6bec4733f2bd47a422444569a9d7a8978cbae1d41552dad0225761678b83f1a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326665"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let fido2Methods = await client.api('/me/authentication/fido2Methods')
    .version('beta')
    .get();

```