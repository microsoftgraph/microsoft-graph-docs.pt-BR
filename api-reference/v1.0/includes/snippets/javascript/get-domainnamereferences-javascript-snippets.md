---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 18896734af886cd22028f37781b36293afdb1f2d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607194"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/domains/{domain-name}/domainNameReferences')
    .get();

```