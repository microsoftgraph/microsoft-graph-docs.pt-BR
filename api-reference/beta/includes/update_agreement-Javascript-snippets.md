---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 29bfcc869bb8e510c4c511ad2dee73f00fd6f4d2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34465661"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const agreement = {
  displayName: "displayName-value",
  isViewingBeforeAcceptanceRequired: true
};

let res = await client.api('/agreements/'id'')
    .version('beta')
    .update({agreement : agreement});

```