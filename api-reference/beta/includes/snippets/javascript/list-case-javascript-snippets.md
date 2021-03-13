---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c8ccc43c130e6aa0146f6e8d6e42910165137fad
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776554"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cases = await client.api('/compliance/ediscovery/cases')
    .version('beta')
    .get();

```