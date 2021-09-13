---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d2cb5f051cd1e6e94a429e579a47d99ee75cd832
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59046132"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/external/connections/contosohr/groups/31bea3d537902000/members/14m1b9c38qe647f6a')
    .delete();

```