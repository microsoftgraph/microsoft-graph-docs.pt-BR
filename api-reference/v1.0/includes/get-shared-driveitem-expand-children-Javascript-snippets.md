---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 077fc33ed89ca63455291b710a27ff5a60420761
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34462573"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/shares/{shareIdOrUrl}/driveItem')
    .expand('children')
    .get();

```