---
title: Tipo de recurso authenticationContext
description: Descreve o contexto de autenticação de acesso condicional de um evento de entrada.
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: c768615d585423f2dd99c95961965d415bde1244
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137232"
---
# <a name="authenticationcontext-resource-type"></a>Tipo de recurso authenticationContext

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve o contexto de autenticação de acesso condicional de um evento de entrada. 

Para obter mais detalhes sobre o contexto de autenticação no acesso condicional, consulte [a documentação de](/azure/active-directory/conditional-access/concept-conditional-access-cloud-apps#authentication-context-preview)contexto de acesso condicional . 

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|detail|authenticationContextDetail|Descreve como o contexto de autenticação de acesso condicional foi acionado. Um valor de significa que o contexto de autenticação ocorreu porque o usuário já satisfez os requisitos para esse contexto de autenticação `previouslySatisfied` em algum evento de autenticação anterior. Um valor de significa que o usuário precisava atender ao requisito de contexto de autenticação `required` como parte do fluxo de login. Os valores possíveis são: `required`, `previouslySatisfied`, `notApplicable`, `unknownFutureValue`.|
|id|Cadeia de caracteres|O identificador de um contexto de autenticação em seu locatário.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.authenticationContext"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationContext",
  "id": "String (identifier)",
  "detail": "String"
}
```

