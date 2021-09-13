---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a5b147a26342ebd863e583163ad65708bfc814aa8898089845821ea6a5999af8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329906"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let externalConnection = await client.api('/connections/contosohr')
    .get();

```