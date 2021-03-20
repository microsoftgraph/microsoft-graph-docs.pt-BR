---
title: Tipo de recurso informationProtectionLabel
description: Descreve o rótulo de proteção de informações que detalha como aplicar corretamente um rótulo de sensibilidade às informações.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 4937d428fd480c0f31a5368a76c4eede9efef851
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953751"
---
# <a name="informationprotectionlabel-resource-type"></a>Tipo de recurso informationProtectionLabel

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve o rótulo de proteção de informações que detalha como aplicar corretamente um rótulo de sensibilidade às informações. O **recurso informationProtectionLabel** descreve a configuração de rótulos de sensibilidade que se aplicam a um usuário ou locatário.  

## <a name="methods"></a>Métodos

| Método                                                                                              | Tipo de retorno                                                               | Descrição                                                                                                                                                            |
| :-------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------ | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Listar informationProtectionLabel](../api/informationprotectionpolicy-list-labels.md)                | [Coleção informationProtectionLabel](informationprotectionlabel.md) | Listar todos os rótulos de proteção de informações configurados para um usuário ou locatário.                                                                                                |
| [Obter informationProtectionLabel](../api/informationprotectionlabel-get.md)                          | [informationProtectionLabel](informationprotectionlabel.md)               | Dada uma ID de rótulo específica, retorne **informationProtectionLabel**.                                                                                                  |
| [evaluateapplication](../api/informationprotectionlabel-evaluateapplication.md)                     | [Coleção informationProtectionAction](informationprotectionaction.md)  | Dada uma entrada [de contentInfo](contentinfo.md) e [labelingOptions](labelingoptions.md), calcule o conjunto de ações necessárias para aplicar o rótulo.                      |
| [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) | [Coleção informationProtectionAction](informationprotectionaction.md)  | Dada uma entrada de [contentInfo](contentinfo.md) e resultados de classificação, calcule o conjunto de ações necessárias para aplicar o rótulo.                                  |
| [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md)                             | [Coleção informationProtectionAction](informationprotectionaction.md)  | Dada uma entrada [de contentInfo](contentinfo.md) e [downgradeJustification](downgradejustification.md), calcule as ações que devem ser tomadas para remover o rótulo. |
| [extractLabel](../api/informationprotectionlabel-extractlabel.md)                                   | [informationProtectionContentLabel](informationprotectioncontentlabel.md) | Dada uma entrada de [contentInfo](contentinfo.md), retorne detalhes sobre [informationProtectionLabel](informationprotectionlabel.md) que os metadados representam.       |

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo    | Descrição                                                                                     |
| :---------- | :------ | :---------------------------------------------------------------------------------------------- |
| color       | String  | A cor que a interface do usuário deve exibir para o rótulo, se configurada.                              |
| description | Cadeia de caracteres  | A descrição definida pelo administrador para o rótulo.                                                    |
| id          | Cadeia de caracteres  | A ID do rótulo é um identificador global exclusivo (GUID)                                             |
| isActive    | Booliano | Indica se o rótulo está ativo ou não. Os rótulos ativos devem ser ocultos ou desabilitados na interface do usuário. |
| nome        | Cadeia de caracteres  | O nome do texto sem formatção do rótulo.                                                                |
| sensibilidade | Int32   | O valor de sensibilidade do rótulo, onde menor é menos sensível.                              |
| tooltip     | Cadeia de caracteres  | A dica de ferramenta que deve ser exibida para o rótulo em uma interface do usuário.                                     |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.informationProtectionLabel",
  "keyProperty": "id"
}-->

```json
{
  "color": "String",
  "description": "String",
  "id": "String (identifier)",
  "isActive": true,
  "name": "String",
  "sensitivity": 1024,
  "tooltip": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "informationProtectionLabel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


