---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 78cb7145df026e29066206d58a6ecffdc06ee12c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084795"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let set = await client.api('/sites/microsoft.sharepoint.com,b9b0bc03-cbc4-40d2-aba9-2c9dd9821ddf,6a742cee-9216-4db5-8046-13a595684e74/termStore/sets/8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f')
    .get();

```