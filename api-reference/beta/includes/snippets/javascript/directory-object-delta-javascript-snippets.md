---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 97a53a11800301d009a319a3f21235a02c77f20f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862435"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryObjects/delta')
    .version('beta')
    .get();

```