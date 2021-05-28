---
title: Tipo de recurso groupSetting
description: As configurações de grupo controlam comportamentos como listas de palavras bloqueadas para nomes de exibição de grupo ou se os usuários convidados têm permissão para serem proprietários do grupo.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 1e18f78f0b0d7c9e8cb9c054afd5645ae45e1c48
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680875"
---
# <a name="groupsetting-resource-type"></a>Tipo de recurso groupSetting

Namespace: microsoft.graph

As configurações de grupo controlam comportamentos como listas de palavras bloqueadas para nomes de exibição de grupo ou se os usuários convidados têm permissão para serem proprietários do grupo.

As configurações de grupo podem ser criadas com base no [groupSettingTemplates](groupsettingtemplate.md)disponível e alteradas de seus padrões predefinidos. Essas configurações governam comportamentos de grupo em um nível de locatário ou em um grupo específico. Quando a mesma configuração é definida em todo o locatário e em um grupo específico, a configuração de nível de grupo substitui a configuração de todo o locatário.  Por exemplo, a configuração de todo o locatário pode permitir que os convidados sejam convidados por membros existentes de grupos, mas uma configuração de grupo individual pode substituir e não permitir que os convidados sejam convidados por membros do grupo. As configurações de grupo governam apenas Microsoft 365 comportamento de grupos.

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Criar configuração](../api/groupsetting-post-groupsettings.md) | [groupSetting](groupsetting.md) |Crie um objeto de configuração com base em um groupSettingTemplate. A solicitação POST deve fornecer settingValues para todas as configurações definidas no modelo. |
|[Obter configuração](../api/groupsetting-get.md) | [groupSetting](groupsetting.md) | Ler propriedades de um objeto de configuração específico. |
|[Listar configurações](../api/groupsetting-list.md) | Conjunto [groupSetting](groupsetting.md) | Lista propriedades de todos os objetos de configuração. |
|[Atualizar configuração](../api/groupsetting-update.md) | [groupSetting](groupsetting.md) | Atualizar objeto groupsetting. |
|[Excluir configuração](../api/groupsetting-delete.md) | Nenhum | Excluir um objeto de configuração. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|displayName|Cadeia de caracteres| Nome de exibição desse grupo de configurações, que vem do modelo associado. |
|id|Cadeia de caracteres| Identificador exclusivo para essas configurações. Somente leitura. |
|templateId|Cadeia de caracteres| Identificador exclusivo do modelo usado para criar esse grupo de configurações. Somente leitura. |
|values|[coleção settingValue](settingvalue.md)| Coleção de pares de valores de nome. Deve conter e definir todas as configurações definidas no modelo. |

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

