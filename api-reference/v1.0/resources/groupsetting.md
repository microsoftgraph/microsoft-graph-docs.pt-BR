---
title: tipo de recurso groupSetting
description: As configurações de grupo controlam comportamentos como listas de palavras bloqueadas para nomes de exibição de grupo ou se os usuários convidados podem ser proprietários de grupo.
ms.openlocfilehash: 16eb67e717fb151a627961176b1409e8426e3178
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004299"
---
# <a name="groupsetting-resource-type"></a>tipo de recurso groupSetting

As configurações de grupo controlam comportamentos como listas de palavras bloqueadas para nomes de exibição de grupo ou se os usuários convidados podem ser proprietários de grupo.

As configurações de grupo podem ser criadas com base no [groupSettingTemplates](groupsettingtemplate.md) disponível e alteradas de seus padrões predefinidos. Essas configurações regem os comportamentos de grupo em um nível total de locatários ou para um grupo específico. Quando a mesma configuração é definida no nível do locatário e para um grupo específico, a configuração de nível de grupo anula a configuração de nível de locatários.  Por exemplo, a configuração de nível de locatário pode permitir que os convidados sejam convidados por membros existentes dos grupos, mas uma configuração de grupo individual pode substitui-la e não permitir que os convidados sejam convidados por membros do grupo. As configurações de grupo regem apenas o comportamento dos grupos do Office 365.

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Criar configuração](../api/groupsetting-post-groupsettings.md) | [groupSetting](groupsetting.md) |Crie um objeto de configuração com base em um groupSettingTemplate. A solicitação POST deve fornecer settingValues para todas as configurações definidas no modelo. |
|[Obter configuração](../api/groupsetting-get.md) | [groupSetting](groupsetting.md) | Ler propriedades de um objeto de configuração específico. |
|[Listar configurações](../api/groupsetting-list.md) | Conjunto [groupSetting](groupsetting.md) | Lista propriedades de todos os objetos de configuração. |
|[Atualizar configuração](../api/groupsetting-update.md) | [groupSetting](groupsetting.md) | Atualize o objeto groupsetting. |
|[Excluir configuração](../api/groupsetting-delete.md) | None | Excluir um objeto de configuração. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|displayName|String| Nome de exibição deste grupo de configurações, originado do modelo associado. |
|id|String| Identificador exclusivo destas configurações. Somente leitura. |
|templateId|String| Identificador exclusivo para o modelo usado para criar este grupo de configurações. Somente leitura. |
|values|conjunto [settingValue](settingvalue.md)| Conjunto de pares de nome/valor. Deve conter e ajustar todas as configurações definidas no modelo. |

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