---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 45d8931542bb86a5d8f82bbfc4d9a6f403ad4a7e8358be4fca3cea3fe2cfe465
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898867"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let authenticationFlowsPolicy = await client.api('/policies/authenticationFlowsPolicy')
    .version('beta')
    .get();

```