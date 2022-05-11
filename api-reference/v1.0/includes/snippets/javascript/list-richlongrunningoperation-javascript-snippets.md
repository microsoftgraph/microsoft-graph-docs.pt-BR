---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e61c4c234de974c7ed8279e4691aea9c5a401736
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65314201"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let list = await client.api('/sites/root/lists/Documents')
    .get();

```