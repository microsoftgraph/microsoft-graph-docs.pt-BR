---
title: Tipo de recurso mfaDetail
description: 'Indica detalhes do MFA para uma assinatura específica. Ele inclui o método de autenticação usado para entrar, bem como detalhes de autenticação (por exemplo: Telefone, SMS ou caixa postal) '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: besiler
ms.openlocfilehash: b3cd2392b9591cfb5465f2f269db547cd37754ea
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50759794"
---
# <a name="mfadetail-resource-type"></a>Tipo de recurso mfaDetail

Namespace: microsoft.graph Indica detalhes de MFA para uma conexão específica. Ele inclui o método de autenticação usado para entrar, bem como detalhes de autenticação (por exemplo: Telefone, SMS ou caixa postal)



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|authDetail|Cadeia de Caracteres|Indica o detalhe de auth MFA para a atividade de Login correspondente quando o MFA Obrigatório é "Sim".|
|authMethod|Cadeia de Caracteres|Indica que os métodos MFA Auth (SMS, Telefone, Aplicativo Autenticador são parte do valor) para a atividade de login correspondente quando o campo MFA Obrigatório for "Sim".|

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


