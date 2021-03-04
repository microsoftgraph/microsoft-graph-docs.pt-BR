---
title: Tipo de recurso directorySetting
description: As configurações de diretório podem ser criadas com base no directorySettingTemplates disponível e alteradas de seus padrões predefinidos.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 50c73e9c68cd3d2fa3f4aed6c7eba84141443d1a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440448"
---
# <a name="directorysetting-resource-type"></a>Tipo de recurso directorySetting

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

As configurações de diretório podem ser criadas com base no [directorySettingTemplates](directorysettingtemplate.md)disponível e alteradas de seus padrões predefinidos. Essas configurações podem reger comportamentos de entidade ou recurso, tanto em um nível de locatário quanto em um nível específico de entidade. Quando a mesma configuração é definida no nível de entidade específica e em todo o locatário, a configuração de nível de entidade específica pode optar pela configuração de todo o locatário.  Por exemplo, a configuração de todo o locatário pode permitir que os convidados sejam convidados por membros existentes de grupos, mas uma configuração de grupo específica pode optar por não permitir que os convidados sejam convidados pelos membros do grupo. Atualmente, as configurações definidas pelo sistema são apenas o comportamento de grupos do Office.

> **Observação**: a versão /beta do tipo de recurso directorySetting só se aplica a grupos. A versão /v1.0 foi renomeada para groupSetting.

## <a name="methods"></a>Methods

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar configuração](../api/directorysetting-post-settings.md) | [directorySetting](directorysetting.md) |Crie um objeto de configuração com base em um directorySettingTemplate. A solicitação POST deve fornecer settingValues para todas as configurações definidas no modelo.|
|[Obter configuração](../api/directorysetting-get.md) | [directorySetting](directorysetting.md) |Ler propriedades de um objeto de configuração específico.|
|[Listar configurações](../api/directorysetting-list.md) | conjunto [directorySetting](directorysetting.md) |Lista propriedades de todos os objetos de configuração.|
|[Atualizar configuração](../api/directorysetting-update.md) | [directorySetting](directorysetting.md)  |Atualizar um objeto setting. Somente settingValues pode ser alterado em uma atualização.|
|[Excluir configuração](../api/directorysetting-delete.md) | Nenhum |Excluir um objeto de configuração. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|displayName|string|Nome de exibição desse grupo de configurações, que vem do modelo associado. Somente leitura.|
|id|string| Identificador exclusivo para essas configurações. Somente leitura.|
|templateId|string| Identificador exclusivo do modelo usado para criar esse grupo de configurações. Somente leitura.|
|values|[coleção settingValue](settingvalue.md)| Coleção de pares de valores de nome. Deve conter e definir todas as configurações definidas no modelo.|

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


