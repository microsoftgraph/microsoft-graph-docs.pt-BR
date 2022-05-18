---
title: Tipo de recurso educationTeamsAppResource
description: Corresponde a um [aplicativo Microsoft Teams instalado](teamsappinstallation.md). Isso permite que os usuários do serviço de educação criem e compartilhem atribuições com aplicativos Teams inseridos.
author: adarshgh
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a3f77be2aa1a5e6566b8d216735138da2daab8c3
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461656"
---
# <a name="educationteamsappresource-resource-type"></a>Tipo de recurso educationTeamsAppResource

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um recurso de educação que corresponde a um [aplicativo Microsoft Teams instalado](teamsappinstallation.md). Isso permite que os usuários do serviço de educação criem e compartilhem atribuições com aplicativos Teams inseridos, como o YouTube ou o FlipGrid.

Para obter informações sobre como usar o FlipGrid para educação Microsoft Teams, consulte [a introdução ao FlipGrid](https://education.microsoft.com/en-us/resource/13cb22b1).

Herda de [educationResource](educationresource.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|displayName|cadeia de caracteres|O nome de exibição do recurso.|
|appId|string|Teams ID do aplicativo.|
|appIconWebUrl|string|URL que aponta para o ícone do aplicativo.|
|teamsEmbeddedContentUrl|string|URL para o recurso de aplicativo que será aberto por Teams.|
|webUrl|cadeia de caracteres|URL para o recurso de aplicativo que pode ser aberto no navegador.|
|createdBy|Cadeia de caracteres|O nome de exibição do usuário que criou esse recurso. Herdado **de educationResource**.|
|createdDateTime|DateTimeOffset|Data em que a reordenação foi adicionada. Herdado **de educationResource**.|
|lastModifiedBy|[identitySet](identityset.md)|O último usuário a modificar o recurso. Herdado **de educationResource**.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que o recurso foi modificado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Herdado **de educationResource**.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTeamsAppResource"
}-->

```json
{
  "displayName": "String",
  "appId": "Unique String",
  "appIconWebUrl": "String URL",
  "teamsEmbeddedContentUrl": "String URL",
  "webUrl": "String URL",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"  
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationExcelResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


