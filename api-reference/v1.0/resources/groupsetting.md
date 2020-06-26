---
title: tipo de recurso groupSetting
description: Os comportamentos de controle de configurações de grupo, como listas de palavras bloqueadas para nomes de exibição de grupo, ou se os usuários convidados podem ser proprietários de grupo.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 162230dc7a197d9f7b927a0b25be734834a5322b
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896928"
---
# <a name="groupsetting-resource-type"></a>tipo de recurso groupSetting

Namespace: microsoft.graph

Os comportamentos de controle de configurações de grupo, como listas de palavras bloqueadas para nomes de exibição de grupo, ou se os usuários convidados podem ser proprietários de grupo.

As configurações de grupo podem ser criadas com base no [groupSettingTemplates](groupsettingtemplate.md)disponível e alteradas de seus padrões predefinidos. Essas configurações controlam os comportamentos de grupo em um nível de locatário ou em um grupo específico. Quando a mesma configuração é definida em todo o locatário e em um grupo específico, a configuração de nível de grupo substitui a configuração em todo o locatário.  Por exemplo, a configuração em todo o locatário pode permitir que convidados sejam convidados por membros existentes de grupos, mas uma configuração de grupo individual pode substituir e não permitir que convidados sejam convidados por membros do grupo. As configurações de grupo controlam o comportamento de grupos do Microsoft 365.

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Criar configuração](../api/groupsetting-post-groupsettings.md) | [groupSetting](groupsetting.md) |Criar um objeto Setting com base em um groupSettingTemplate. A solicitação POST deve fornecer settingValues para todas as configurações definidas no modelo. |
|[Obter configuração](../api/groupsetting-get.md) | [groupSetting](groupsetting.md) | Ler propriedades de um objeto de configuração específico. |
|[Listar configurações](../api/groupsetting-list.md) | Conjunto [groupSetting](groupsetting.md) | Lista propriedades de todos os objetos de configuração. |
|[Atualizar configuração](../api/groupsetting-update.md) | [groupSetting](groupsetting.md) | Atualize o objeto groupsetting. |
|[Excluir configuração](../api/groupsetting-delete.md) | None | Excluir um objeto de configuração. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|displayName|Cadeia de caracteres| Exibe o nome deste grupo de configurações, que vem do modelo associado. |
|id|String| Identificador exclusivo dessas configurações. Somente leitura. |
|templateId|String| Identificador exclusivo para o modelo usado para criar esse grupo de configurações. Somente leitura. |
|values|coleção [SettingValue](settingvalue.md)| Coleção de pares de valor de nome. Deve conter e definir todas as configurações definidas no modelo. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.groupSetting"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "templateId": "String",
  "values": [{"@odata.type": "microsoft.graph.settingValue"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
