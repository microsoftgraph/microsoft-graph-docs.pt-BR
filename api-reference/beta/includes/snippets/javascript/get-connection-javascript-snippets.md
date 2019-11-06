---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 146944b96fb641241902072956ec6bcf2bec1840
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994665"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/connections/contosohr')
    .version('beta')
    .get();

```