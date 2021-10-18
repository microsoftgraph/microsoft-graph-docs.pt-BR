---
title: Tipo de recurso requiredResourceAccess
description: Especifica o conjunto de escopos de permissão OAuth 2.0 e funções de aplicativo.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 374d88cd9cc0166c003618af4382aafe498eaf87
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60452829"
---
# <a name="requiredresourceaccess-resource-type"></a>Tipo de recurso requiredResourceAccess

Namespace: microsoft.graph

Especifica o conjunto de escopos de permissão OAuth 2.0 e funções de aplicativo sob o recurso especificado ao que um aplicativo requer acesso. O [aplicativo](application.md) pode solicitar os escopos de permissão ou funções de aplicativo OAuth 2.0 especificados por meio da propriedade **requiredResourceAccess,** que é uma coleção de objetos [requiredResourceAccess.](requiredresourceaccess.md)

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|resourceAccess|[coleção resourceAccess](resourceaccess.md)|A lista de escopos de permissão OAuth2.0 e funções de aplicativo que o aplicativo exige do recurso especificado.|
|resourceAppId|Cadeia de caracteres|O identificador exclusivo do recurso ao que o aplicativo requer acesso. Isso deve ser igual ao **appId** declarado no aplicativo de recurso de destino.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requiredResourceAccess"
}-->

```json
{
  "resourceAccess": [
    {
      "@odata.type": "microsoft.graph.resourceAccess"
    }
  ],
  "resourceAppId": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "requiredResourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

