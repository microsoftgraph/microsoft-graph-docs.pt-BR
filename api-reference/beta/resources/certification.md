---
title: tipo de recurso de certificação
description: Representa os detalhes de certificação de um aplicativo.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: arpitha-dhanapathi
ms.openlocfilehash: 6dedb9b58e3b59c707c6601fea12e9751ec3026f
ms.sourcegitcommit: 3e2239e60b6dc53997b7d4356a20fc3d365d6238
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/02/2021
ms.locfileid: "61266422"
---
# <a name="certification-resource-type"></a>tipo de recurso de certificação

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de certificação de um [aplicativo](application.md). 

A propriedade de certificação de um aplicativo é somente leitura e não pode ser definida manualmente. Ele é atualizado quando o aplicativo é certificado por meio do programa Microsoft 365 conformidade de aplicativos. Para obter mais informações, [consulte Microsoft 365 App Compliance Program](/microsoft-365-app-certification/docs/enterprise-app-certification-guide).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|certificationDetailsUrl|String|URL que mostra detalhes de certificação para o aplicativo.|
|certificationExpirationDateTime|DateTimeOffset|O timestamp quando a certificação atual do aplicativo expirará.|
|isCertifiedByMicrosoft|Boolean|Indica se o aplicativo é certificado pela Microsoft.|
|isPublisherAttested|Boolean|Indica se o aplicativo foi autotestado pelo desenvolvedor de aplicativos ou pelo editor.|
|lastCertificationDateTime|DateTimeOffset|O timestamp quando a certificação do aplicativo foi adicionada ou atualizada mais recentemente.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.certification"
}-->

```json
{
  "isPublisherAttested": "Boolean",
  "isCertifiedByMicrosoft": "Boolean",
  "certificationDetailsUrl": "String",
  "lastCertificationDateTime": "DateTimeOffset",
  "certificationExpirationDateTime": "DateTimeOffset"
}
```
