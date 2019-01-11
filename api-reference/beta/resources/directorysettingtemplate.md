---
title: tipo de recurso de directorySettingTemplate
description: Modelos de configuração de diretório representam as configurações definidas pelo sistema disponíveis para o inquilino. Configurações do diretório podem ser criadas com base nos directorySettingTemplates disponíveis e valores alterados de seus padrões predefinidas. Modelos de configuração do diretório não podem ser criados, atualizados ou excluídos. Essas configurações podem representar as configurações de todo o locatário, ou podem representar as configurações de entidade específica.  Atualmente, os únicos modelos disponíveis se aplicam a grupos do Office e incluem configurações como se os usuários podem criar grupos ou convidar pessoas de fora da organização para se tornar membros de um grupo.
localization_priority: Normal
ms.openlocfilehash: e0df923854059723ee83380f7aa0f6425cf2afb9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806143"
---
# <a name="directorysettingtemplate-resource-type"></a>tipo de recurso de directorySettingTemplate

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Modelos de configuração de diretório representam as configurações definidas pelo sistema disponíveis para o inquilino. [Configurações do diretório](directorysetting.md) podem ser criados com base nos directorySettingTemplates disponíveis e valores alterados de seus padrões predefinidas. Modelos de configuração do diretório não podem ser criados, atualizados ou excluídos. Essas configurações podem representar as configurações de todo o locatário, ou podem representar as configurações de entidade específica.  Atualmente, os únicos modelos disponíveis se aplicam a grupos do Office e incluem configurações como se os usuários podem criar grupos ou convidar pessoas de fora da organização para se tornar membros de um grupo.

> **Observação**: A versão /beta do tipo de recurso directorySettingTemplate se aplica apenas aos grupos. A versão /v1.0 foi renomeada para groupSettingTemplate.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter directorySettingTemplate](../api/directorysettingtemplate-get.md) | [directorySettingTemplate](directorysettingtemplate.md) |Leia as propriedades específicas de um dos objetos directorySettingTemplate definidas pelo sistema.|
|[Lista directorySettingTemplate](../api/directorysettingtemplate-list.md) | [Coleção de directorySettingTemplate](directorysettingtemplate.md) |Liste todos os objetos directorySettingTemplate definidas pelo sistema.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|description|string|Descrição do modelo. Somente leitura.|
|displayName|string|Nome para exibição do modelo Somente leitura. |
|id|string| O identificador exclusivo do modelo. Somente leitura.|
|values|Conjunto [settingTemplateValue](settingtemplatevalue.md)| Coleção de settingTemplateValues que lista o conjunto de configurações disponíveis, padrões e tipos que compõem este modelo.  Somente leitura. |

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
<!-- {
  "type": "#page.annotation",
  "description": "directorySettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
