---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 03870f78d536e1c1318440ec77107a8b253e1aac21d415f2959f45b8f62d9dad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099381"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let b2xUserFlows = await client.api('/identity/b2xUserFlows')
    .version('beta')
    .expand('identityProviders')
    .get();

```