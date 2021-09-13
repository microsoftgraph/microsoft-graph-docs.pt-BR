---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c973c87e63ad12f65b4ec76828999f7f759219b4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59147556"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/sites/{site-id}/contentTypes/{contentType-id}')
    .delete();

```