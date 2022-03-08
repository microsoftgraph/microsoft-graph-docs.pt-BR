---
title: Tipo de recurso directorySetting
description: As configurações de diretório podem ser criadas com base no directorySettingTemplates disponível e alteradas de seus padrões predefinidos.
ms.localizationpriority: medium
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: eb442e80e92b746e864507536b0e0b0992e8cd9a
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335273"
---
# <a name="directorysetting-resource-type"></a>Tipo de recurso directorySetting

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

As configurações de diretório definem as configurações que podem ser usadas para personalizar as restrições específicas do locatário e do objeto e o comportamento permitido. Por exemplo, você pode bloquear listas de palavras para nomes de exibição de grupo ou definir se os usuários convidados têm permissão para serem proprietários do grupo.

Por padrão, todas as entidades herdam os padrões predefinidos. Para alterar as configurações padrão, você deve criar um novo objeto de configuração usando [o directorySettingTemplates](directorysettingtemplate.md). Quando a mesma configuração é definida em todo o locatário e em um grupo específico, a configuração de nível de entidade substitui a configuração em todo o locatário. Por exemplo, a configuração de todo o locatário pode permitir que os convidados sejam convidados por membros existentes de grupos, mas uma configuração de grupo individual pode substituir e não permitir que os convidados sejam convidados por membros do grupo.

> [!TIP]
> A `/v1.0` versão desse recurso é chamada [groupSetting](/graph/api/resources/groupsetting?view=graph-rest-1.0&preserve-view=true).

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar configuração](../api/group-post-settings.md) | [directorySetting](directorysetting.md) |Crie um objeto de configuração com base em um directorySettingTemplate.|
|[Obter configuração](../api/directorysetting-get.md) | [directorySetting](directorysetting.md) |Ler propriedades de um objeto de configuração específico.|
|[Listar configurações](../api/group-list-settings.md) | conjunto [directorySetting](directorysetting.md) |Lista propriedades de todos os objetos de configuração.|
|[Atualizar configuração](../api/directorysetting-update.md) | [directorySetting](directorysetting.md)  |Atualizar um objeto setting. Somente settingValues pode ser alterado em uma atualização.|
|[Excluir configuração](../api/directorysetting-delete.md) | Nenhum |Excluir um objeto de configuração. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|displayName|string|Nome de exibição desse grupo de configurações, que vem do modelo associado. Somente leitura.|
|id|string| Identificador exclusivo para essas configurações. Somente leitura.|
|templateId|string| Identificador exclusivo do modelo usado para criar esse grupo de configurações. Somente leitura.|
|values|[coleção settingValue](settingvalue.md)| Coleção de pares de valores de nome correspondentes ao nome e propriedades defaultValue no objeto [directorySettingTemplates](directorysettingtemplate.md) referenciado.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySetting"
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "templateId": "string",
  "values": [{"@odata.type": "microsoft.graph.settingValue"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directorySetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


