---
title: Tipo de recurso directorySettingTemplate
description: Os modelos de configuração de diretório representam configurações definidas pelo sistema disponíveis para o locatário.
ms.localizationpriority: medium
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 372abab6126a9e2174638fd59fceb609f6f072c3
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335231"
---
# <a name="directorysettingtemplate-resource-type"></a>Tipo de recurso directorySettingTemplate

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os modelos de configuração de diretório representam configurações definidas pelo sistema disponíveis para o locatário. [As configurações de](directorysetting.md) diretório podem ser criadas com base nos **directorySettingTemplates** disponíveis e valores alterados de seus padrões predefinidos. Modelos de configuração de diretório não podem ser criados, atualizados ou excluídos. Essas configurações podem representar configurações de todo o locatário ou podem representar configurações de entidade específicas. Atualmente, os únicos modelos disponíveis para grupos se aplicam Microsoft 365 grupos e incluem configurações como se os usuários podem criar grupos ou convidar convidados de fora da organização para se tornarem membros de um grupo.

Para obter mais informações sobre as configurações Microsoft 365 de grupo disponíveis, consulte [Configurações de modelo](/azure/active-directory/enterprise-users/groups-settings-cmdlets).

> [!TIP]
> A `/v1.0` versão desse recurso é chamada [groupSettingTemplate](/graph/api/resources/groupsettingtemplate?view=graph-rest-1.0&preserve-view=true).

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter directorySettingTemplate](../api/directorysettingtemplate-get.md) | [directorySettingTemplate](directorysettingtemplate.md) |Leia as propriedades específicas de um dos objetos directorySettingTemplate definidos pelo sistema.|
|[Listar directorySettingTemplate](../api/directorysettingtemplate-list.md) | [Coleção de directorySettingTemplate](directorysettingtemplate.md) |Listar todos os objetos directorySettingTemplate definidos pelo sistema.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|description|string|Descrição do modelo. Somente leitura.|
|displayName|string|Nome de exibição do modelo. Somente leitura. |
|id|string| Identificador exclusivo do modelo. Somente leitura.|
|values|[Coleção settingTemplateValue](settingtemplatevalue.md)| Coleção de settingTemplateValues que lista o conjunto de configurações, padrões e tipos disponíveis que comem esse modelo.  Somente leitura. |

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySettingTemplate"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "values": [{"@odata.type": "microsoft.graph.settingTemplateValue"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directorySettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


