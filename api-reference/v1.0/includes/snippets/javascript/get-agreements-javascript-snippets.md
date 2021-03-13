---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fd51d74b69e1e06fdfacf2a2c05dc5f742e65b47
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775203"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let agreements = await client.api('/identityGovernance/termsOfUse/agreements')
    .get();

```