---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 744cf49083aa9091e1e3a5286db8244cf6870e46
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50966744"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookTableCollectionPage tables = graphClient.me().drive().items("{id}").workbook().tables()
    .buildRequest()
    .get();

```