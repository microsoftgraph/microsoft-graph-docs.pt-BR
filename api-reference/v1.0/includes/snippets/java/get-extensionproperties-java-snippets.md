---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2bcfee2a3e0c8b68c8bcfc3ba25acd87051c3adf
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37999143"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IExtensionPropertyCollectionPage extensionProperties = graphClient.applications("{id}").extensionProperties()
    .buildRequest()
    .get();

```