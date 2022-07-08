---
title: teamTemplateDefinition
description: Representação genérica de uma definição de modelo de equipe para uma equipe com uma estrutura e configuração específicas.
author: Charlieforce
ms.localizationpriority: medium
ms.prod: teamwork
doc_type: resourcePageType
ms.openlocfilehash: 9df396be7eca713cd407c253af8285528e6587f8
ms.sourcegitcommit: c168f2cb95b4863080a84cc199a7b878fb5eeb8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2022
ms.locfileid: "66690095"
---
# <a name="teamtemplatedefinition-resource-type"></a>Tipo de recurso teamTemplateDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representação genérica de uma definição de modelo de equipe para uma equipe com uma estrutura e configuração específicas.

Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter teamTemplateDefinition](../api/teamtemplatedefinition-get.md)|[teamTemplateDefinition](../resources/teamtemplatedefinition.md)|Leia as propriedades e as relações de um [objeto teamTemplateDefinition](../resources/teamtemplatedefinition.md) .|
| [Listar teamTemplateDefinitions](../api/teamtemplate-list-definitions.md) | [Coleção teamTemplateDefinition](../resources/teamtemplatedefinition.md) | Liste **os objetos teamTemplateDefinition** associados a um **teamTemplate**.  |
| [Obter teamDefinition](../api/teamtemplatedefinition-get-teamdefinition.md) | [equipe](../resources/team.md) | Ler as propriedades da **equipe de** um **objeto teamTemplateDefinition** |

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Público|teamTemplateAudience|Descreve o público-alvo para o qual o modelo de equipe está disponível. Os valores possíveis são: `organization`, `user`, `public`, `unknownFutureValue`.|
|categories|String collection|As categorias atribuídas para o modelo de equipe.|
|descrição|Cadeia de caracteres|Uma breve descrição do modelo de equipe como ele aparecerá para os usuários no Microsoft Teams.|
|displayName|Cadeia de caracteres|O nome definido pelo usuário do modelo de equipe.|
|iconUrl|Cadeia de Caracteres|A URL do ícone do modelo de equipe.|
|id|Cadeia de caracteres|Codificado64 do modelo `templateId` +  + `audience``locale` de equipe. Herdado da [entidade](../resources/entity.md).|
|languageTag|Cadeia de caracteres|Idioma em que o modelo está disponível.|
|lastModifiedBy|[identitySet](../resources/identityset.md)|A identidade do usuário que modificou o modelo de equipe pela última vez.|
|lastModifiedDateTime|DateTimeOffset|A data em que o modelo de equipe foi modificado pela última vez.|
|parentTemplateId|Cadeia de Caracteres|O `templateId` modelo de equipe|
|publisherName|String|A organização que publicou o modelo de equipe.|
|Shortdescription|Cadeia de Caracteres|Uma breve descrição do modelo de equipe como ele aparecerá para os usuários no Microsoft Teams.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|teamDefinition|[equipe](../resources/team.md)|Coleção de objetos [de](../resources/channel.md) canal. Um canal representa um tópico e, portanto, um isolamento lógico da discussão em uma equipe.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamtemplatedefinition",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamTemplateDefinition",
  "id": "String (identifier)",
  "parentTemplateId": "String",
  "displayName": "String",
  "languageTag": "String",
  "audience": "String",
  "description": "String",
  "shortDescription": "String",
  "iconUrl": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "publisherName": "String",
  "categories": [
    "String"
  ]
}
```
## <a name="see-also"></a>Confira também

- [equipe](team.md)
- [teamsTemplate](teamsTemplate.md)
