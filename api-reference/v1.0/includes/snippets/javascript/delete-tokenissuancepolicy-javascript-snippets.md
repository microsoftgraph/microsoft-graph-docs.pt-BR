---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b06e18f5b940d42f00224eb7da53967544f30df7b47bb2e28a7ee9b1e1518484
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56900273"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/tokenIssuancePolicies/{id}')
    .delete();

```