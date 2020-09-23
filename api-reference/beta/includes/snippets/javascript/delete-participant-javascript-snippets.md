---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 536447395ad04afda534a94c7cd2d36745b84e00
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48222876"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/communications/calls/{id}/participants/{id}')
    .version('beta')
    .delete();

```