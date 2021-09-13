---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 309971d8ac0407942689e2cc60c20d48969e2c7d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59022478"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/external/connections/contosohr/groups/31bea3d537902000')
    .delete();

```