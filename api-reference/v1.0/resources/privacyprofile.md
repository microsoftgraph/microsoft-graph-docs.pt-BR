---
title: Tipo de recurso privacyProfile
description: Representa o perfil de privacidade de uma empresa que inclui uma URL da política de privacidade e uma pessoa de contato para tirar dúvidas sobre a política de privacidade.
localization_priority: Normal
ms.openlocfilehash: 29c4a01cde0e05c42ce74576e769ca005840e854
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884977"
---
# <a name="privacyprofile-resource-type"></a>Tipo de recurso privacyProfile

Representa o perfil de privacidade de uma empresa que inclui uma URL da política de privacidade e uma pessoa de contato para tirar dúvidas sobre a política de privacidade.

## <a name="properties"></a>Propriedades
| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|contactEmail|Cadeia de caracteres| Um endereço de email smtp válido para o contato da política de privacidade. Não obrigatório.|
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
