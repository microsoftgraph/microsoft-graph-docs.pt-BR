---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 91090cb22b94c1211c267eefe1f3e9169b31e1704845b81cf40fbdfb672057ca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099317"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let availableProviderTypes = await client.api('/identityProviders/availableProviderTypes')
    .get();

```