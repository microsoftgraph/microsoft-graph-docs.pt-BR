---
title: Tipo de recurso directorySettingTemplate
description: Os modelos de configuração de diretório representam configurações definidas pelo sistema disponíveis para o locatário.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 71984d472aab9f78197134fae0668fd0a90d7716
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440406"
---
# <a name="directorysettingtemplate-resource-type"></a>Tipo de recurso directorySettingTemplate

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os modelos de configuração de diretório representam configurações definidas pelo sistema disponíveis para o locatário. [As configurações de](directorysetting.md) diretório podem ser criadas com base nos directorySettingTemplates disponíveis e valores alterados de seus padrões predefinidos. Modelos de configuração de diretório não podem ser criados, atualizados ou excluídos. Essas configurações podem representar configurações de todo o locatário ou podem representar configurações de entidade específicas.  Atualmente, os únicos modelos disponíveis se aplicam a grupos do Office e incluem configurações como se os usuários podem criar grupos ou convidar convidados de fora da organização para se tornarem membros de um grupo.

> **Observação**: a versão /beta do tipo de recurso directorySettingTemplate só se aplica a grupos. A versão /v1.0 foi renomeada para groupSettingTemplate.

## <a name="methods"></a>Methods

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


