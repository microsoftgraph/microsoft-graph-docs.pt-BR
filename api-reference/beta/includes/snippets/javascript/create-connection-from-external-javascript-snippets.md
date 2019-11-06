---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 60cd9c42645e0b1d19dd27e409a2710d32173215
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994722"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const externalConnection = {
  id: "contosohr",
  name: "Contoso HR",
  description: "Connection to index Contoso HR system"
};

let res = await client.api('/external/connections')
    .version('beta')
    .post(externalConnection);

```