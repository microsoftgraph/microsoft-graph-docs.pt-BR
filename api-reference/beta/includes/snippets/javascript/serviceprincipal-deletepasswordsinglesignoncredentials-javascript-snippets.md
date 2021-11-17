---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b695966d2553610ab54fdda0bdac3c8e95ef2324700782504b92efdd62d93c69
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215545"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const deletePasswordSingleSignOnCredentials = {
  id: '5793aa3b-cca9-4794-679a240f8b58'
};

await client.api('/servicePrincipals/{id}/deletePasswordSingleSignOnCredentials')
    .version('beta')
    .post(deletePasswordSingleSignOnCredentials);

```