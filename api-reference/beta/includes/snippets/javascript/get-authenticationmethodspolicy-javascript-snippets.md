---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4a6c1c71f5f320f935238a101e1b2562e96096a445101b08d8feb96b214c59b8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157482"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let authenticationMethodsPolicy = await client.api('/policies/authenticationMethodsPolicy')
    .version('beta')
    .get();

```