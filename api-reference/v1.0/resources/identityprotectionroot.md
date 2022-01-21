---
title: Tipo de recurso identityProtectionRoot
description: Contêiner para propriedades de navegação para recursos Graph proteção de identidade da Microsoft.
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 1d1ea31820743a0c132ee5f179b0917900a32e1a
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/21/2022
ms.locfileid: "62161982"
---
# <a name="identityprotectionroot-resource-type"></a>Tipo de recurso identityProtectionRoot

Namespace: microsoft.graph

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

