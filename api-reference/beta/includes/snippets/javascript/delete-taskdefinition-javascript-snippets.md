---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a9035c6872eca5d7c896e654b662061ece8c82fe0adfad2483eaa5e407d586c7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101583"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/taskDefinitions/4c6a0f26-8e5d-4bf6-91e6-4a5731adec19')
    .version('beta')
    .delete();

```