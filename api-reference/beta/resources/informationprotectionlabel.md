---
title: tipo de recurso informationProtectionLabel
description: Descreve o rótulo de proteção de informações que detalha como aplicar corretamente um rótulo de confidencialidade às informações.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 528238d904ac9807027dd51a8c59ed03570c7bc3
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938741"
---
# <a name="informationprotectionlabel-resource-type"></a>tipo de recurso informationProtectionLabel

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve o rótulo de proteção de informações que detalha como aplicar corretamente um rótulo de confidencialidade às informações. O recurso **informationProtectionLabel** descreve a configuração de rótulos de confidencialidade que se aplicam a um usuário ou locatário.  

## <a name="methods"></a>Métodos

| Método                                                                                              | Tipo de retorno                                                               | Descrição                                                                                                                                                            |
| :-------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------ | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Listar informationProtectionLabel](../api/informationprotectionpolicy-list-labels.md)                | coleção [informationProtectionLabel](informationprotectionlabel.md) | Listar todos os rótulos de proteção de informações configurados para um usuário ou locatário.                                                                                                |
| [Obter informationProtectionLabel](../api/informationprotectionlabel-get.md)                          | [informationProtectionLabel](informationprotectionlabel.md)               | Dada uma ID de etiqueta específica, retorne o **informationProtectionLabel**.                                                                                                  |
| [evaluateapplication](../api/informationprotectionlabel-evaluateapplication.md)                     | coleção [informationProtectionAction](informationprotectionaction.md)  | Dada uma entrada de [contentInfo](contentinfo.md) e [labelingOptions](labelingoptions.md), COMPUTE o conjunto de ações necessárias para aplicar o rótulo.                      |
| [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) | coleção [informationProtectionAction](informationprotectionaction.md)  | Dada uma entrada de [contentInfo](contentinfo.md) e resultados de classificação, COMPUTE o conjunto de ações necessárias para aplicar o rótulo.                                  |
| [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md)                             | coleção [informationProtectionAction](informationprotectionaction.md)  | Dada uma entrada de [contentInfo](contentinfo.md) e [downgradeJustification](downgradejustification.md), calcule as ações que devem ser executadas para remover o rótulo. |
| [extractLabel](../api/informationprotectionlabel-extractlabel.md)                                   | [informationProtectionContentLabel](informationprotectioncontentlabel.md) | Dada uma entrada de [contentInfo](contentinfo.md), detalhes de retorno no [informationProtectionLabel](informationprotectionlabel.md) que os metadados representam.       |

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo    | Descrição                                                                                     |
| :---------- | :------ | :---------------------------------------------------------------------------------------------- |
| color       | String  | A cor que a interface do usuário deve exibir para o rótulo, se configurada.                              |
| description | Cadeia de caracteres  | A descrição definida pelo administrador para o rótulo.                                                    |
| id          | String  | A ID do rótulo é um identificador global exclusivo (GUID)                                             |
| isActive    | Booliano | Indica se o rótulo está ativo ou não. Os rótulos ativos devem ser ocultos ou desabilitados na interface do usuário. |
| name        | Cadeia de caracteres  | O nome de texto não criptografado do rótulo.                                                                |
| sensitivity | Int32   | O valor de confidencialidade do rótulo, onde inferior é menos confidencial.                              |
| tooltip     | String  | A dica de ferramenta que deve ser exibida para o rótulo em uma interface do usuário.                                     |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.informationProtectionLabel",
  "baseType": "",
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
