---
title: tipo de recurso groupSettingTemplate
description: Modelos de configuração de grupo representam configurações definidas pelo sistema disponíveis para o locatário.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 0d1d1359a515d854b71fab5b01792d1e31843343
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896921"
---
# <a name="groupsettingtemplate-resource-type"></a>tipo de recurso groupSettingTemplate

Namespace: microsoft.graph

Modelos de configuração de grupo representam configurações definidas pelo sistema disponíveis para o locatário. [As configurações de grupo](groupsetting.md) podem ser criadas com base no **groupSettingTemplates**disponível e os valores alterados de seus padrões predefinidos. Modelos de configuração de grupo não podem ser criados, atualizados ou excluídos. Essas configurações podem representar configurações de todo o locatário ou podem representar configurações de grupo específicas. Atualmente, os únicos modelos disponíveis se aplicam aos grupos do Microsoft 365 e incluem configurações como se os usuários podem criar grupos ou convidar convidados de fora da organização para se tornarem membros de um grupo.

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Obter groupSettingTemplate](../api/groupsettingtemplate-get.md) | [groupSettingTemplate](groupsettingtemplate.md) | Leia as propriedades específicas de um dos objetos groupSettingTemplate definidos pelo sistema. |
|[Listar groupSettingTemplate](../api/groupsettingtemplate-list.md) | [Coleção de groupSettingTemplate](groupsettingtemplate.md) |Lista todos os objetos groupSettingTemplate definidos pelo sistema.|

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|description|String| Descrição do modelo. |
|displayName|Cadeia de caracteres| Nome para exibição do modelo. |
|id|String| Identificador exclusivo do modelo. Somente leitura.|
|values|coleção [settingTemplateValue](settingtemplatevalue.md)| Coleção de settingTemplateValues que lista o conjunto de configurações disponíveis, padrões e tipos que compõem esse modelo. |

## <a name="relationships"></a>Relações

Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.groupSettingTemplate"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "values": [{"@odata.type": "microsoft.graph.settingTemplateValue"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupSettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
