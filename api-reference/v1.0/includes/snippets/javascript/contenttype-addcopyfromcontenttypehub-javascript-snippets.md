---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8174090daf218320b90a78aa5115d535268b9bf4
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315916"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contentType = {
  contentTypeId: '0x0101'
};

await client.api('/sites/root/lists/Documents/contentTypes/addCopyFromContentTypeHub')
    .post(contentType);

```