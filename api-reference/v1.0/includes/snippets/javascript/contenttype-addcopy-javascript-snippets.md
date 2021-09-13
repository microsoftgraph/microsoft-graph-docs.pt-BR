---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b2669a832bc125fa80a472fe80810edd4e7d77f3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59147695"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contentType = {
  contentType: 'https://graph.microsoft.com/v1.0/sites/{site-id}/contentTypes/0x0101'
};

await client.api('/sites/{site-id}/lists/{list-id}/contentTypes/addCopy')
    .post(contentType);

```