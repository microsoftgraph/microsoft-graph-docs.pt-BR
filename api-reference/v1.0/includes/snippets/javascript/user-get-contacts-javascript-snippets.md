---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a96f521e11529a05d9626305a75a3ea521793c6f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797525"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contacts = await client.api('/me/contacts')
    .get();

```