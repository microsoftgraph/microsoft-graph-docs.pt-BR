---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 927b382c3d56f577b571a443bd391c0d78c006af
ms.sourcegitcommit: 3834b7b0287ee71668c52c42d3465ca19366e678
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2020
ms.locfileid: "43082119"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/contacts/delta')
    .select('displayName,jobTitle,mail')
    .get();

```