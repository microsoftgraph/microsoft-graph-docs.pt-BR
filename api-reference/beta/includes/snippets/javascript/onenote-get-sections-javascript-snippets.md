---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 24c451257ba51eb7655991d063bfad758aa5d372
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878794"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/sections')
    .version('beta')
    .get();

```