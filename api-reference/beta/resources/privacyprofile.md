---
title: Tipo de recurso privacyProfile
description: Representa o perfil de privacidade de uma empresa que inclui uma URL da política de privacidade e uma pessoa de contato para tirar dúvidas sobre a política de privacidade.
localization_priority: Normal
ms.openlocfilehash: d1d7593e5b0f0ef9d4ac36f902ec244e93fd51c1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344197"
---
# <a name="privacyprofile-resource-type"></a>Tipo de recurso privacyProfile

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o perfil de privacidade de uma empresa que inclui uma URL da política de privacidade e uma pessoa de contato para tirar dúvidas sobre a política de privacidade.

## <a name="properties"></a>Propriedades
| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|contactEmail|String| Um endereço de email smtp válido para o contato da política de privacidade. Não necessário.|
|statementUrl|Cadeia de caracteres| Um formato de URL válido começando por http:// ou https://. O tamanho máximo é de 255 caracteres. A URL que direciona para a política de privacidade da empresa. Não obrigatório.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privacyProfile"
}-->

```json
{
  "contactEmail": "string",
  "statementUrl": "string"
}
```
