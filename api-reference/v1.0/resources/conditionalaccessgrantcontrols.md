---
title: Tipo de recurso conditionalAccessGrantControls
description: Representa controles de concessão que devem ser atendidos para passar a política.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 99b6d6dc3bd15ea84c4a8507981acd9c8ac2eb6f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130785"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a>Tipo de recurso conditionalAccessGrantControls

Namespace: microsoft.graph

Representa controles de concessão que devem ser atendidos para passar a política.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-------- |:---- |:----------- |
| operator | String | Define a relação dos controles de concessão. Valores possíveis: `AND` , `OR` . |
| builtInControls | String collection | Lista de valores de controles internos exigidos pela política. Valores possíveis: `block` , , , , , `mfa` `compliantDevice` `domainJoinedDevice` `approvedApplication` `compliantApplication` `passwordChange` . |
| customAuthenticationFactors | String collection | Lista de IDs de controles personalizados exigidas pela política. Para obter mais informações, consulte [Controles personalizados.](/azure/active-directory/conditional-access/controls) |
| termsOfUse | String collection | Lista de [IDs de](/graph/api/resources/agreement) termos de uso exigida pela política. |

### <a name="special-considerations-when-using-passwordchange-as-a-control"></a>Considerações especiais ao usar `passwordChange` como um controle

Considere o seguinte ao usar o `passwordChange` controle: 

- `passwordChange` deve ser acompanhado pelo `mfa` uso de um `AND` operador. Essa combinação garante que a senha seja atualizada de maneira segura.
- `passwordChange` deve ser usado em uma política que contém `userRiskLevels` . Isso foi projetado para permitir cenários em que os usuários devem usar uma senha de alteração segura para redefinir seus riscos de usuário.
- A política deve direcionar `all` aplicativos e não excluir aplicativos.
- A política não pode conter nenhuma outra condição, exceto `users` e `applications` `userRiskLevels` .

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "operator",
    "builtInControls",
    "customAuthenticationFactors",
    "termsOfUse"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessGrantControls",
  "baseType": null
}-->

```json
{
  "builtInControls": ["String"],
  "customAuthenticationFactors": ["String"],
  "operator": "String",
  "termsOfUse": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessGrantControls resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
