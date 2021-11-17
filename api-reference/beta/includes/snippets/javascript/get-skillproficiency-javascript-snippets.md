---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6dafe750eca1e083c6ba38b8ba32f2308e25aa0ec62f11ea2595786316b2b429
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217294"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let skillProficiency = await client.api('/me/profile/skills/{id}')
    .version('beta')
    .get();

```