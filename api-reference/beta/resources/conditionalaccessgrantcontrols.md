---
title: Tipo de recurso conditionalAccessGrantControls
description: Representa os controles de concessão que devem ser cumpridos para passar a política.
ms.localizationpriority: medium
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 68346c835acb3ad46353fe4a48f6a426861484c8
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59763622"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a>Tipo de recurso conditionalAccessGrantControls

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os controles de concessão que devem ser cumpridos para passar a política.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-------- |:---- |:----------- |
| operator | String | Define a relação dos controles de concessão. Valores possíveis: `AND` , `OR` . |
| builtInControls | Coleção conditionalAccessGrantControl | Lista de valores de controles internos exigidos pela política. Valores possíveis: `block` , , , , , , , `mfa` `compliantDevice` `domainJoinedDevice` `approvedApplication` `compliantApplication` `passwordChange` `unknownFutureValue` . |
| customAuthenticationFactors | Coleção de cadeias de caracteres | Lista de IDs de controles personalizados exigidas pela política. Para saber mais sobre controle personalizado, consulte [Controles personalizados (visualização)](/azure/active-directory/conditional-access/controls#custom-controls-preview). |
| termsOfUse | Coleção de cadeias de caracteres | Lista de [termos de](agreement.md) IDs de uso exigidos pela política. |

### <a name="special-considerations-when-using-passwordchange-as-a-control"></a>Considerações especiais ao usar `passwordChange` como um controle

Considere o seguinte ao usar o `passwordChange` controle: 

- `passwordChange` deve ser acompanhado pelo `mfa` uso de um `AND` operador. Essa combinação garante que a senha seja atualizada de forma segura.
- `passwordChange` deve ser usado em uma política que contenha `userRiskLevels` . Isso foi projetado para habilitar cenários em que os usuários devem usar uma senha de alteração segura para redefinir seus riscos de usuário.
- A política deve direcionar `all` aplicativos e não excluir aplicativos.
- A política não pode conter nenhuma outra condição.

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


