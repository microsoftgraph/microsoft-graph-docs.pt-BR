---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 384e0fa1ce86d0f8237c016dc69a8ce7263c93cd465a53cfa0196fc4a60f0e88
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899555"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let applicationTemplates = await client.api('/applicationTemplates')
    .get();

```