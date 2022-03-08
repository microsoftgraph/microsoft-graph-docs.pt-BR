---
title: Tipo de recurso groupSettingTemplate
description: Os modelos de configuração de grupo representam as configurações definidas pelo sistema disponíveis para o locatário.
ms.localizationpriority: medium
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 6da14127e3253b9f23b75997cb0e73cc5b05deb4
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333887"
---
# <a name="groupsettingtemplate-resource-type"></a>Tipo de recurso groupSettingTemplate

Namespace: microsoft.graph

Os modelos de configuração de grupo representam as configurações definidas pelo sistema disponíveis para o locatário. [As configurações de grupo](groupsetting.md) podem ser criadas com base no **groupSettingTemplates** disponível e valores alterados de seus padrões predefinidos. Modelos de configuração de grupo não podem ser criados, atualizados ou excluídos. Essas configurações podem representar configurações de todo o locatário ou representar configurações de grupo específicas. Atualmente, os únicos modelos disponíveis para grupos se aplicam Microsoft 365 grupos e incluem configurações como se os usuários podem criar grupos ou convidar convidados de fora da organização para se tornarem membros de um grupo.

Para obter mais informações sobre as configurações Microsoft 365 de grupo disponíveis, consulte [Configurações de modelo](/azure/active-directory/enterprise-users/groups-settings-cmdlets).

> [!TIP]
> A `/beta` versão desse recurso é chamada [directorySettingTemplate](/graph/api/resources/directorysettingtemplate?view=graph-rest-beta&preserve-view=true).

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Obter groupSettingTemplate](../api/groupsettingtemplate-get.md) | [groupSettingTemplate](groupsettingtemplate.md) | Leia as propriedades específicas de um dos objetos groupSettingTemplate definidos pelo sistema. |
|[Listar groupSettingTemplate](../api/groupsettingtemplate-list.md) | [Coleção de groupSettingTemplate](groupsettingtemplate.md) |Listar todos os objetos groupSettingTemplate definidos pelo sistema.|

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|description|String| Descrição do modelo. |
|displayName|Cadeia de caracteres| Nome de exibição do modelo. O modelo nomeado `Group.Unified` pode ser usado para configurar configurações de grupo em todo o Microsoft 365 de locatários, `Group.Unified.Guest` enquanto o modelo nomeado pode ser usado para configurar configurações específicas do grupo.|
|id|String| Identificador exclusivo do modelo. Somente leitura.|
|values|[Coleção settingTemplateValue](settingtemplatevalue.md)| Coleção de settingTemplateValues que lista o conjunto de configurações, padrões e tipos disponíveis que comem esse modelo. |

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

