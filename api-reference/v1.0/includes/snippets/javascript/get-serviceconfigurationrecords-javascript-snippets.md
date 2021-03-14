---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a51d194639ebec0d601ed1fa2e391cc946491a28
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798531"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let serviceConfigurationRecords = await client.api('/domains/{domain-name}/serviceConfigurationRecords')
    .get();

```