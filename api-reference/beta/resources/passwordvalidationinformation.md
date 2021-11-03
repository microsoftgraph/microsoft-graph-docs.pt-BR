---
title: Tipo de recurso passwordValidationInformation
description: Expõe as propriedades que especificam se a senha de um usuário é válida quando validada em relação à política de validação de senha do locatário.
author: yyuank
ms.localizationpriority: medium
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 0da72df7551b84284dc9caa7d9183ef31834eba7
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60689209"
---
# <a name="passwordvalidationinformation-resource-type"></a>Tipo de recurso passwordValidationInformation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Expõe as propriedades que especificam se a senha de um usuário é válida, quando validada em relação à política de validação de senha do locatário. Esse recurso também retorna a lista de regras nas quais a senha foi validada e se a senha do usuário passou essas funções.


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|isValid|Booliano| Especifica se a senha é válida com base no cálculo dos resultados na **propriedade validationResults.** Não anulável. Somente leitura. |
|validationResults|[Coleção validationResult](../resources/validationresult.md)| A lista de regras de validação de senha e se a senha passou essas regras. Não anulável. Somente leitura. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.passwordValidationInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.passwordValidationInformation",
  "isValid": "Boolean",
  "validationResults": [
    {
      "@odata.type": "microsoft.graph.validationResult"
    }
  ]
}
```

