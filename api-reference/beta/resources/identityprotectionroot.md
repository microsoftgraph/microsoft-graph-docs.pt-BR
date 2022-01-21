---
title: Tipo de recurso identityProtectionRoot
description: Contêiner para propriedades de navegação para recursos Graph proteção de identidade da Microsoft.
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f42dbebc085bcce8f03155e89d440d610d5e1aa1
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/21/2022
ms.locfileid: "62162193"
---
# <a name="identityprotectionroot-resource-type"></a>Tipo de recurso identityProtectionRoot

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contêiner para as propriedades de navegação para recursos Graph proteção de identidade da Microsoft.

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades

Nenhum.

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|riskDetections|[Coleção riskDetection](../resources/riskdetection.md)| Detecção de risco na Proteção de Identidade do Azure AD e as informações associadas sobre a detecção.|
|riskyUsers|[Coleção riskyUser](../resources/riskyuser.md)|Usuários que são sinalizados como em risco pela Proteção de Identidade do Azure AD. |

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

