---
title: Tipo de recurso identityProtectionRoot
description: Contêiner para propriedades de navegação para recursos Graph proteção de identidade da Microsoft.
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 90b8de67f24c650f1a4f6832979f5d669f9af57e
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519444"
---
# <a name="identityprotectionroot-resource-type"></a>Tipo de recurso identityProtectionRoot

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contêiner para as propriedades de navegação [para recursos Graph proteção de identidade da Microsoft](identityprotection-overview.md).

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades

Nenhum.

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|riskDetections|[Coleção riskDetection](../resources/riskdetection.md)| Detecção de risco na Proteção de Identidade do Azure AD e as informações associadas sobre a detecção.|
|riskyUsers|[Coleção riskyUser](../resources/riskyuser.md)|Usuários que são sinalizados como em risco pela Proteção de Identidade do Azure AD. |
|riskyServicePrincipals| [Coleção riskyServicePrincipal](riskyserviceprincipal.md) | Entidades de serviço do Azure AD que estão em risco. |
|servicePrincipalRiskDetections| [Coleção servicePrincipalRiskDetection](serviceprincipalriskdetection.md) | Representa informações sobre entidades de serviço de risco detectadas em um locatário do Azure AD.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityProtectionRoot",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.identityProtectionRoot"
}
```

