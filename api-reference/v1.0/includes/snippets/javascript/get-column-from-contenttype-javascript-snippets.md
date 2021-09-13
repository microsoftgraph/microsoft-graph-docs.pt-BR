---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 268483c724aad372f6cdc427e8c7eff00fe1f182
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59080150"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let columnDefinition = await client.api('/sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}')
    .get();

```