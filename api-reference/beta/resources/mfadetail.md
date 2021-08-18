---
title: Tipo de recurso mfaDetail
description: 'Indica detalhes do MFA para uma assinatura específica. Ele inclui o método de autenticação usado para entrar, bem como detalhes de autenticação (por exemplo: Telefone, SMS ou caixa postal) '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: besiler
ms.openlocfilehash: 52cf5f15c31502fd796e581f8b45e8d00b80eeb83939d7bb6b3c70d6c4906ef2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54249696"
---
# <a name="mfadetail-resource-type"></a>Tipo de recurso mfaDetail

Namespace: microsoft.graph Indica detalhes de MFA para uma conexão específica. Ele inclui o método de autenticação usado para entrar, bem como detalhes de autenticação (por exemplo: Telefone, SMS ou caixa postal)



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|authDetail|Cadeia de caracteres|Indica o detalhe de auth MFA para a atividade de Login correspondente quando o MFA Obrigatório é "Sim".|
|authMethod|Cadeia de caracteres|Indica que os métodos MFA Auth (SMS, Telefone, Authenticator App são parte do valor) para a atividade de login correspondente quando o campo MFA Obrigatório for "Sim".|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mfaDetail"
}-->

```json
{
  "authDetail": "String",
  "authMethod": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mfaDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


