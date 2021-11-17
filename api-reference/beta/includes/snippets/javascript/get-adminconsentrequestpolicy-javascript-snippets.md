---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f743a3ab8f9dd961ea721abe6c215cb6747580d4dcb5fe55533ee45aacfa5ce2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898110"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let adminConsentRequestPolicy = await client.api('/policies/adminConsentRequestPolicy')
    .version('beta')
    .get();

```