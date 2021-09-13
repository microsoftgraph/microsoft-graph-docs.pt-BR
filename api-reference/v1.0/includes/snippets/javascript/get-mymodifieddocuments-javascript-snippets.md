---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ad1ffeef43e7daceaf3b1cd055046b488c69b34534738498f79c5c259f5125ab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102994"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let used = await client.api('/me/insights/used')
    .get();

```