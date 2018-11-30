---
title: tipo de recurso de requiredResourceAccess
description: Especifica o conjunto de escopos de permissão de OAuth 2.0 e funções de aplicativo em que um aplicativo requer acesso ao recurso especificado. Os escopos de permissão especificados OAuth 2.0 podem ser solicitados por aplicativos do cliente (por meio da coleção **requiredResourceAccess** ) quando um aplicativo de recurso de chamada. A propriedade **requiredResourceAccess** da entidade do aplicativo é uma coleção de **ReqiredResourceAccess**.
ms.openlocfilehash: 937557f2f078ade1b336cfd00cd128d428d59cbb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039187"
---
# <a name="requiredresourceaccess-resource-type"></a>tipo de recurso de requiredResourceAccess

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Especifica o conjunto de escopos de permissão de OAuth 2.0 e funções de aplicativo em que um aplicativo requer acesso ao recurso especificado. Os escopos de permissão especificados OAuth 2.0 podem ser solicitados por aplicativos do cliente (por meio da coleção **requiredResourceAccess** ) quando um aplicativo de recurso de chamada. A propriedade **requiredResourceAccess** da entidade do [aplicativo](application.md) é uma coleção de **ReqiredResourceAccess**.


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
  "resourceAccess": [{"@odata.type": "microsoft.graph.resourceAccess"}],
  "resourceAppId": "string"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|resourceAccess|Coleção [ResourceAccess](resourceaccess.md)|A lista de escopos de permissão OAuth2.0 e funções de aplicativo que requer que o aplicativo do recurso especificado.|
|resourceAppId|String|O identificador exclusivo para o recurso que o aplicativo exija acesso à.  Este deve ser igual a **appId** declaradas na aplicação de recurso de destino.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "requiredResourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
