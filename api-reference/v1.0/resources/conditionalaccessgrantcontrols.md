---
title: Tipo de recurso conditionalAccessGrantControls
description: Representa os controles de concessão que devem ser cumpridos para passar a política.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 6bd2c8dbcd6a57b9f97d810e5691cb2c705c67d2cf322a7b3d26369aa57489dd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54223631"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a>Tipo de recurso conditionalAccessGrantControls

Namespace: microsoft.graph

Representa os controles de concessão que devem ser cumpridos para passar a política.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-------- |:---- |:----------- |
| operator | Cadeia de caracteres | Define a relação dos controles de concessão. Valores possíveis: `AND` , `OR` . |
| builtInControls | Coleção conditionalAccessGrantControl | Lista de valores de controles internos exigidos pela política. Valores possíveis: `block` , , , , , , , `mfa` `compliantDevice` `domainJoinedDevice` `approvedApplication` `compliantApplication` `passwordChange` `unknownFutureValue` . |
| customAuthenticationFactors | Coleção de cadeias de caracteres | Lista de IDs de controles personalizados exigidas pela política. Para obter mais informações, consulte [Controles personalizados](/azure/active-directory/conditional-access/controls). |
| termsOfUse | Coleção de cadeias de caracteres | Lista de [termos de](/graph/api/resources/agreement) IDs de uso exigidos pela política. |

### <a name="special-considerations-when-using-passwordchange-as-a-control"></a>Considerações especiais ao usar `passwordChange` como um controle

Considere o seguinte ao usar o `passwordChange` controle: 

- `passwordChange` deve ser acompanhado pelo `mfa` uso de um `AND` operador. Essa combinação garante que a senha seja atualizada de forma segura.
- `passwordChange` deve ser usado em uma política que contenha `userRiskLevels` . Isso foi projetado para habilitar cenários em que os usuários devem usar uma senha de alteração segura para redefinir seus riscos de usuário.
- A política deve direcionar `all` aplicativos e não excluir aplicativos.
- A política não pode conter nenhuma outra condição, exceto `users` , `applications` e `userRiskLevels` .

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
