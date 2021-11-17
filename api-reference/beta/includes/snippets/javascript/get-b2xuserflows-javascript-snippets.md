---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 057a9b227fb870e03aa3e3aa40c2edf260db9eba7f80bc789b837a639de6191f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101638"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let b2xIdentityUserFlow = await client.api('/identity/b2xUserFlows/{id}')
    .version('beta')
    .get();

```