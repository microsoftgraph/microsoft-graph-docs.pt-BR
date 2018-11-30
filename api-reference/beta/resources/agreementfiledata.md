---
title: tipo de recurso de agreementFileData
description: Representa o blob do Azure Active Directory termos (Azure AD) do arquivo do contrato de uso.
ms.openlocfilehash: 557725e14f4954f8b2c10112e1013beb71dda0be
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037062"
---
# <a name="agreementfiledata-resource-type"></a>tipo de recurso de agreementFileData

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa o blob do Azure Active Directory termos (Azure AD) do arquivo do contrato de uso.

## <a name="properties"></a>Propriedades
| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
|data|Binário|Dados que representam as condições de usar o documento PDF. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFileData"
}-->

```json
{
  "data": "Binary"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "agreementFileData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
