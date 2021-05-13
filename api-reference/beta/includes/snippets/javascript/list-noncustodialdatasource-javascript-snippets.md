---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ec5b1b67425e5820cb0967cba391cbc1a0ead609
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52476724"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let noncustodialDataSources = await client.api('/compliance/ediscovery/cases/5b840b94-f821-4c4a-8cad-3a90062bf51a/noncustodialDataSources')
    .version('beta')
    .get();

```