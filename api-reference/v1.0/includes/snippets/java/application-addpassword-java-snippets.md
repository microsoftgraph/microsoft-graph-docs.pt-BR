---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 47a33fdfbc4473ced91a807ddfc5b5854632a751
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "37999429"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PasswordCredential passwordCredential = new PasswordCredential();
passwordCredential.displayName = "Password friendly name";

graphClient.applications("{id}")
    .addPassword(passwordCredential)
    .buildRequest()
    .post();

```