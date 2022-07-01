---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 456a04e988af5fea194a014b54d1fee679c08f4e
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2022
ms.locfileid: "66577906"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/reports/getM365AppUserCounts(period='D7')')
    .version('beta')
    .get();

```