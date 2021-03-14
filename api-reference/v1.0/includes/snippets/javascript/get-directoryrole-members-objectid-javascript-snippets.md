---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7505cc4edef710c4b506450c2f9f18da3987a167
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793521"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/directoryRoles/23f3b4b4-8a29-4420-8052-e4950273bbda/members')
    .get();

```