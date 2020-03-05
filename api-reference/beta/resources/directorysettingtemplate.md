---
title: tipo de recurso directorySettingTemplate
description: Modelos de configuração de diretório representam configurações definidas pelo sistema disponíveis para o locatário. As configurações de diretório podem ser criadas com base no directorySettingTemplates disponível e os valores alterados de seus padrões predefinidos. Os modelos de configuração de diretório não podem ser criados, atualizados ou excluídos. Essas configurações podem representar configurações de todo o locatário ou podem representar configurações específicas da entidade.  Atualmente, os únicos modelos disponíveis se aplicam aos grupos do Office e incluem configurações como se os usuários podem criar grupos ou convidar convidados de fora da organização para se tornarem membros de um grupo.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f1881c697eae6b4032635d2e4797a14ef2e848e2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42506460"
---
# <a name="directorysettingtemplate-resource-type"></a>tipo de recurso directorySettingTemplate

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Modelos de configuração de diretório representam configurações definidas pelo sistema disponíveis para o locatário. [As configurações de diretório](directorysetting.md) podem ser criadas com base no directorySettingTemplates disponível e os valores alterados de seus padrões predefinidos. Os modelos de configuração de diretório não podem ser criados, atualizados ou excluídos. Essas configurações podem representar configurações de todo o locatário ou podem representar configurações específicas da entidade.  Atualmente, os únicos modelos disponíveis se aplicam aos grupos do Office e incluem configurações como se os usuários podem criar grupos ou convidar convidados de fora da organização para se tornarem membros de um grupo.

> **Observação**: a versão do/beta do tipo de recurso directorySettingTemplate só se aplica a grupos. A versão do/v1.0 foi renomeada como groupSettingTemplate.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter directorySettingTemplate](../api/directorysettingtemplate-get.md) | [directorySettingTemplate](directorysettingtemplate.md) |Leia as propriedades específicas de um dos objetos directorySettingTemplate definidos pelo sistema.|
|[Listar directorySettingTemplate](../api/directorysettingtemplate-list.md) | [Coleção de directorySettingTemplate](directorysettingtemplate.md) |Lista todos os objetos directorySettingTemplate definidos pelo sistema.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|description|string|Descrição do modelo. Somente leitura.|
|displayName|cadeia de caracteres|Nome para exibição do modelo. Somente leitura. |
|id|string| Identificador exclusivo do modelo. Somente leitura.|
|values|coleção [settingTemplateValue](settingtemplatevalue.md)| Coleção de settingTemplateValues que lista o conjunto de configurações disponíveis, padrões e tipos que compõem esse modelo.  Somente leitura. |

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
