---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f685a0f203cec8227b0e15c5b0072c335598e9829c3caece4653fbbacc351643
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214059"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tiIndicators = await client.api('/security/tiIndicators')
    .version('beta')
    .get();

```