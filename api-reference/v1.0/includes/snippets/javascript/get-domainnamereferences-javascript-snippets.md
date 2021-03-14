---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ac7da217cf4694766b208544ab2b6ed682c9c0c5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780893"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let domainNameReferences = await client.api('/domains/{domain-name}/domainNameReferences')
    .get();

```