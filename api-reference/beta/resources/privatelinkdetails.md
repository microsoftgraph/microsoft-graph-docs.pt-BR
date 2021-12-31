---
title: Tipo de recurso privateLinkDetails
description: Fornece detalhes sobre Links Privados no locatário do Azure AD
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 8392b9a1a0e86a1f12a17d96c3fa7e8d06f7437b
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647207"
---
# <a name="privatelinkdetails-resource-type"></a>Tipo de recurso privateLinkDetails

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece detalhes sobre o Link Privado do Azure associado a um evento de login. Para obter mais informações sobre o Link Privado do Azure, consulte [O que é o Link Privado do Azure?](/azure/private-link/private-link-overview) 



## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|policyId|String|O identificador exclusivo da política de Link Privado. |
|policyName|String|O nome da política de Link Privado no Azure AD. |
|policyTenantId|String|O identificador de locatário do locatário do Azure AD ao que a política de Link Privado pertence.|
|resourceId|Cadeia de caracteres|O caminho do Gerenciador de Recursos do Azure (ARM) para o recurso de política de Link Privado.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.privateLinkDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.privateLinkDetails",
  "policyId": "String",
  "policyName": "String",
  "resourceId": "String",
  "policyTenantId": "String"
}
```
