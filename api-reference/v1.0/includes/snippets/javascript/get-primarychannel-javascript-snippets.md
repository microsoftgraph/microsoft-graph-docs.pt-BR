---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e8bf9a5bfec849e4f8197133c513b2b0fce1cdf8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808622"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let channel = await client.api('/teams/{id}/primaryChannel')
    .get();

```