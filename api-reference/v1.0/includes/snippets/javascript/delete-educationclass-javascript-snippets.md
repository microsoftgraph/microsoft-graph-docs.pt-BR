---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ed89a573fe2c919a111ba1feca363a2f108e1ece9ed280307ba0201c348ec8ba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57375788"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/classes/{class-id}')
    .delete();

```