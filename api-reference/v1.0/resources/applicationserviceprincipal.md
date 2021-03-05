---
title: Tipo de recurso applicationServicePrincipal
description: Uma combinação de um aplicativo e um servicePrincipal.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 35abee6b3028111ce4237828b58492a546ff5d4b
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50476411"
---
# <a name="applicationserviceprincipal-resource-type"></a>Tipo de recurso applicationServicePrincipal

Namespace: microsoft.graph

Quando uma instância de um aplicativo da galeria de aplicativos do Azure AD é adicionada, os objetos [application](../resources/application.md) e [servicePrincipal](../resources/serviceprincipal.md) são criados no diretório. O **applicationServicePrincipal** representa a concatenação do **objeto** application e **servicePrincipal.**

## <a name="methods"></a>Métodos

Nenhum

## <a name="properties"></a>Propriedades

| Propriedade         | Tipo                                                 | Descrição                                                     |
| :--------------- | :--------------------------------------------------- | :-------------------------------------------------------------- |
| application      | [aplicativo](../resources/application.md)           | Representa um aplicativo registrado no Azure Active Directory. |
| servicePrincipal | [servicePrincipal](../resources/serviceprincipal.md) | Representa uma instância de um aplicativo em um diretório.        |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationServicePrincipal",
  "keyProperty": "id"
}-->

```json
{
  "servicePrincipal": { "@odata.type": "microsoft.graph.servicePrincipal" },
  "application": { "@odata.type": "microsoft.graph.application" }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationServicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
