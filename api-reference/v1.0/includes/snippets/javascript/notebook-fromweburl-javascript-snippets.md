---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 79ebd9c7471430b523be7b5e2d9edd9f42624977
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793165"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const copyNotebookModel = {webUrl: 'webUrl value'};

await client.api('/me/onenote/notebooks/GetNotebookFromWebUrl')
    .post(copyNotebookModel);

```