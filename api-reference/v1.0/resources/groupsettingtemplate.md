---
title: tipo de recurso groupSettingTemplate
description: Os modelos de configuração de grupo representam configurações definidas pelo sistema disponíveis para o locatário. As configurações de grupo podem ser criadas com base no **groupSettingTemplates** disponível e valores alterados de seus padrões predefinidos. Os modelos de configuração de grupo não podem ser criados, atualizados ou excluídos. Essas configurações podem representar configurações de nível de locatário ou configurações de grupo específico. Atualmente, os únicos modelos disponíveis se aplicam aos grupos do Office 365 e incluem as configurações, como se os usuários podem criar grupos ou convidar pessoas de fora da organização a se tornarem membros de um grupo.
ms.openlocfilehash: 3c4111b2727e79e048778063b259611795733de4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006992"
---
# <a name="groupsettingtemplate-resource-type"></a>tipo de recurso groupSettingTemplate

Os modelos de configuração de grupo representam configurações definidas pelo sistema disponíveis para o locatário. As [configurações de grupo](groupsetting.md) podem ser criadas com base no **groupSettingTemplates** disponível e valores alterados de seus padrões predefinidos. Os modelos de configuração de grupo não podem ser criados, atualizados ou excluídos. Essas configurações podem representar configurações de nível de locatário ou configurações de grupo específico. Atualmente, os únicos modelos disponíveis se aplicam aos grupos do Office 365 e incluem as configurações, como se os usuários podem criar grupos ou convidar pessoas de fora da organização a se tornarem membros de um grupo.

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Obter groupSettingTemplate](../api/groupsettingtemplate-get.md) | [groupSettingTemplate](groupsettingtemplate.md) | Leia as propriedades específicas de um dos objetos groupSettingTemplate definidos pelo sistema. |
|[Lista groupSettingTemplate](../api/groupsettingtemplate-list.md) | [Coleção de groupSettingTemplate](groupsettingtemplate.md) |Lista todos os objetos de groupSettingTemplate definidos pelo sistema.|

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|description|String| Descrição do modelo. |
|displayName|String| Nome para exibição do modelo |
|id|String| O identificador exclusivo do modelo. Somente leitura.|
|values|Conjunto [settingTemplateValue](settingtemplatevalue.md)| Coleção de settingTemplateValues que lista o conjunto de configurações disponíveis, padrões e tipos que compõem este modelo. |

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