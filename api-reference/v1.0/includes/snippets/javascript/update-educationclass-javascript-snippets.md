---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: be6fd6f3a857c6048afb7a09089086f3eaae886caa612f6379bb12bab8d34543
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327542"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationClass = {
  description: 'History - World History 1',
  displayName: 'World History Level 1',
};

await client.api('/education/classes/{class-id}')
    .update(educationClass);

```