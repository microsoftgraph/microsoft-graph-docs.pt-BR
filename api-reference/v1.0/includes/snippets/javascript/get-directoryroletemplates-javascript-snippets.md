---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8cc2a36df4923164a03f1aee68235c33e6aea331
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48617384"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryRoleTemplates')
    .get();

```