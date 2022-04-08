---
title: Tipo de recurso delegatedAdminRelationshipCustomerParticipant
description: Representa detalhes de identificação de um cliente em uma relação de administrador delegado.
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: resourcePageType
ms.openlocfilehash: 228681c0ade8f7b0db7ad3901e402049288cefd7
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704421"
---
# <a name="delegatedadminrelationshipcustomerparticipant-resource-type"></a>Tipo de recurso delegatedAdminRelationshipCustomerParticipant

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa detalhes de identificação de um cliente em uma relação de administrador delegado.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome de exibição do locatário do cliente conforme definido pelo Azure AD. Somente leitura|
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

