---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 815ef94c9c09f71e2bb35dff9eedd2a0f589437f
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474952"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let classes = await client.api('/education/classes')
    .get();

```