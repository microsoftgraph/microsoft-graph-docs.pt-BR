---
title: tipo de recurso delegatedAdminRelationshipCustomerParticipant
description: Representa os detalhes de identificação de um cliente em uma relação de administrador delegada.
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 738ae13f0a999cecc7d1b24bb5ef2fec81302441
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589530"
---
# <a name="delegatedadminrelationshipcustomerparticipant-resource-type"></a>tipo de recurso delegatedAdminRelationshipCustomerParticipant

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de identificação de um cliente em uma relação de administrador delegada.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome de exibição do locatário do cliente conforme definido pelo Azure AD. Somente leitura|
|tenantId|String|A ID de locatário atribuída ao Azure AD do locatário do cliente.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.delegatedAdminRelationshipCustomerParticipant"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.delegatedAdminRelationshipCustomerParticipant",
  "tenantId": "String",
  "displayName": "String"
}
```

