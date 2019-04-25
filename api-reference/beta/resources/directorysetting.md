---
title: tipo de recurso directorySetting
description: As configurações de diretório podem ser criadas com base no directorySettingTemplates disponível e alteradas de seus padrões predefinidos. Essas configurações podem controlar comportamentos de entidade ou de recurso, tanto em um nível de locatário quanto em um nível de entidade específico. Quando a mesma configuração é definida no nível de entidade de todo o locatário e específico, a configuração de nível de entidade específica pode ser recusada a partir da configuração de todo o locatário.  Por exemplo, a configuração de todos os locatários pode permitir que convidados sejam convidados por membros existentes de grupos, mas uma configuração de grupo específico pode recusar e não permitir que convidados sejam convidados por membros do grupo. As configurações definidas pelo sistema atualmente são controlar o comportamento de grupos do Office.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b489bf1130bd91d28b3a2b41a78c38b881e90d27
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535220"
---
# <a name="directorysetting-resource-type"></a>tipo de recurso directorySetting

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

As configurações de diretório podem ser criadas com base no [directorySettingTemplates](directorysettingtemplate.md)disponível e alteradas de seus padrões predefinidos. Essas configurações podem controlar comportamentos de entidade ou de recurso, tanto em um nível de locatário quanto em um nível de entidade específico. Quando a mesma configuração é definida no nível de entidade de todo o locatário e específico, a configuração de nível de entidade específica pode ser recusada a partir da configuração de todo o locatário.  Por exemplo, a configuração de todos os locatários pode permitir que convidados sejam convidados por membros existentes de grupos, mas uma configuração de grupo específico pode recusar e não permitir que convidados sejam convidados por membros do grupo. As configurações definidas pelo sistema atualmente são controlar o comportamento de grupos do Office.

> **Observação**: a versão do/beta do tipo de recurso directorySetting só se aplica a grupos. A versão do/v1.0 foi renomeada como groupSetting.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar configuração](../api/directorysetting-post-settings.md) | [directorySetting](directorysetting.md) |Criar um objeto Setting com base em um directorySettingTemplate. A solicitação POST deve fornecer settingValues para todas as configurações definidas no modelo.|
|[Obter configuração](../api/directorysetting-get.md) | [directorySetting](directorysetting.md) |Ler propriedades de um objeto de configuração específico.|
|[Listar configurações](../api/directorysetting-list.md) | conjunto [directorySetting](directorysetting.md) |Lista propriedades de todos os objetos de configuração.|
|[Atualizar configuração](../api/directorysetting-update.md) | [directorySetting](directorysetting.md)  |Atualizar um objeto setting. Somente settingValues pode ser alterado em uma atualização.|
|[Excluir configuração](../api/directorysetting-delete.md) | None |Excluir um objeto de configuração. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|displayName|string|Exibe o nome deste grupo de configurações, que vem do modelo associado. Somente leitura.|
|id|string| Identificador exclusivo dessas configurações. Somente leitura.|
|templateId|string| Identificador exclusivo para o modelo usado para criar esse grupo de configurações. Somente leitura.|
|values|[](settingvalue.md) coleção SettingValue| Coleção de pares de valor de nome. Deve conter e definir todas as configurações definidas no modelo.|

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
  "suppressions": [
    "Error: /api-reference/beta/resources/directorysetting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
