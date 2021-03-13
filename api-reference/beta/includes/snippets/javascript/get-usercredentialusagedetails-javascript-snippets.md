---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b33097220446fda74df9b38352eefd235f00ff00
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809326"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userCredentialUsageDetails = await client.api('/reports/userCredentialUsageDetails')
    .version('beta')
    .get();

```