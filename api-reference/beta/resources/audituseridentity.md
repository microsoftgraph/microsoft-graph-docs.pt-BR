---
title: Tipo de recurso auditUserIdentity
description: Um tipo aberto que representa detalhes da identidade de um usuário juntamente com informações sobre seu locatário de residência.
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: fc3d4f2de96c878184d38ed3eae4bf795875e35f
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647200"
---
# <a name="audituseridentity-resource-type"></a>Tipo de recurso auditUserIdentity

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um tipo aberto que representa detalhes da identidade de um usuário juntamente com informações sobre seu locatário de residência.

Herda de [userIdentity](../resources/useridentity.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome de exibição do usuário. Herdado da [identidade](../resources/identity.md).|
|homeTenantId|String|Para entrar no usuário, o identificador do locatário de que o usuário é membro.|
|homeTenantName|String|Para entrar no usuário, o nome do locatário de que o usuário é membro. Somente populado em casos em que o locatário da residência forneceu consentimento afirmativo ao Azure AD para mostrar o conteúdo do locatário.|
|id|String|Identificador exclusivo do usuário. Herdado da [identidade](../resources/identity.md).|
|ipAddress|Cadeia de caracteres|O endereço IP do Azure AD detectado para o cliente do usuário. Herdado [de userIdentity](../resources/useridentity.md).|
|userPrincipalName|String|Upn (Nome de Entidade de Usuário) do usuário. Herdado [de userIdentity](../resources/useridentity.md).|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditUserIdentity",
  "baseType": "microsoft.graph.userIdentity",
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditUserIdentity",
  "displayName": "String",
  "id": "String (identifier)",
  "ipAddress": "String",
  "userPrincipalName": "String",
  "homeTenantId": "String",
  "homeTenantName": "String"
}
```

