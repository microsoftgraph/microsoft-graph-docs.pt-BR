---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3b888d6ac9586acd6a6f33cc8490a83b5f1cc5b64547ba72b93864473fd8bb1a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099296"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let monthlyPrintUsageByPrinter = await client.api('/reports/monthlyPrintUsageByPrinter')
    .get();

```