---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2bd79a292c0b0435678673b32bd6a2881da4e1dd
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612575"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directorySettingTemplates')
    .version('beta')
    .get();

```