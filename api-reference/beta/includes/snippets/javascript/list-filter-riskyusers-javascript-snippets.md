---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4feadb8c0c288051f88e9e0b7df7b06898cf41af99487d91c7a277a5efdd7139
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157052"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let riskyUsers = await client.api('/identityProtection/riskyUsers')
    .version('beta')
    .filter('riskLevel eq microsoft.graph.riskLevel\'medium\'')
    .get();

```