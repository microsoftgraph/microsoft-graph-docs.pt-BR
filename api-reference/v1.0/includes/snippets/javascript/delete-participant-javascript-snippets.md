---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eee3cd74a75f2aab6b86e9192c6dfed39d739f6134bba9d6332547c11cce1acf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275133"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/communications/calls/{id}/participants/{id}')
    .delete();

```