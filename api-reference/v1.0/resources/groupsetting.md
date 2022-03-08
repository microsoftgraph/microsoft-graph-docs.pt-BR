---
title: Tipo de recurso groupSetting
description: As configurações de grupo definem as configurações que podem ser usadas para personalizar as restrições específicas do locatário e do objeto e o comportamento permitido. Por exemplo, você pode bloquear listas de palavras para nomes de exibição de grupo ou definir se os usuários convidados têm permissão para serem proprietários do grupo.
author: Jordanndahl
ms.localizationpriority: medium
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 17e535c8584d6e9364257220eadc1aebba9c540b
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337429"
---
# <a name="groupsetting-resource-type"></a>Tipo de recurso groupSetting

Namespace: microsoft.graph

As configurações de grupo definem as configurações que podem ser usadas para personalizar as restrições específicas do locatário e do objeto e o comportamento permitido. Por exemplo, você pode bloquear listas de palavras para nomes de exibição de grupo ou definir se os usuários convidados têm permissão para serem proprietários do grupo.

Por padrão, todos os grupos herdam os padrões predefinidos. Para alterar as configurações padrão, você deve criar um novo objeto de configuração usando [o groupSettingTemplates](groupsettingtemplate.md). Quando a mesma configuração é definida em todo o locatário e em um grupo específico, a configuração de nível de grupo substitui a configuração de todo o locatário. Por exemplo, a configuração de todo o locatário pode permitir que os convidados sejam convidados por membros existentes de grupos, mas uma configuração de grupo individual pode substituir e não permitir que os convidados sejam convidados por membros do grupo.

As configurações de grupo se aplicam apenas Microsoft 365 grupos.

> [!TIP]
> A `/beta` versão desse recurso é chamada [directorySetting](/graph/api/resources/directorysetting?view=graph-rest-beta&preserve-view=true).

## <a name="methods"></a>Methods

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Criar configuração](../api/group-post-settings.md) | [groupSetting](groupsetting.md) |Crie um objeto de configuração com base em **um groupSettingTemplate**.|
|[Obter configuração](../api/groupsetting-get.md) | [groupSetting](groupsetting.md) | Ler propriedades de um objeto de configuração específico. |
|[Listar configurações](../api/group-list-settings.md) | Conjunto [groupSetting](groupsetting.md) | Lista propriedades de todos os objetos de configuração. |
|[Atualizar configuração](../api/groupsetting-update.md) | [groupSetting](groupsetting.md) | Atualizar objeto groupsetting. |
|[Excluir configuração](../api/groupsetting-delete.md) | Nenhum | Excluir um objeto de configuração. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|displayName|String| Nome de exibição desse grupo de configurações, que vem do modelo associado. |
|id|Cadeia de caracteres| Identificador exclusivo para essas configurações. Somente leitura. |
|templateId|Cadeia de caracteres| Identificador exclusivo para o objeto [groupSettingTemplates](groupsettingtemplate.md) no nível de locatário que foi personalizado para este objeto de configurações de nível de grupo. Somente leitura. |
|values|[coleção settingValue](settingvalue.md)| Coleção de pares de valores de nome correspondentes ao **nome** e propriedades **defaultValue** no objeto [groupSettingTemplates](groupsettingtemplate.md) referenciado. |

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

