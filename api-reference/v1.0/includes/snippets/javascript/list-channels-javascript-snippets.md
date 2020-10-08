---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a9837f3f644031111acdbd735dfc4ad9111f0584
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373597"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/channels')
    .get();

```