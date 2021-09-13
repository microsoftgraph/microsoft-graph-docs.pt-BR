---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b59513e339d60fbc9697f32e9e1d921e00d23a30
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59038193"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let _boolean = await client.api('/sites/{siteId}/contentTypes/{contentTypeId}/isPublished')
    .get();

```