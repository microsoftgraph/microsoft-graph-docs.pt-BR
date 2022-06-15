---
title: tipo de recurso de certificação
description: Representa os detalhes de certificação de um aplicativo.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: arpitha-dhanapathi
ms.openlocfilehash: 228670677eb8d618803bb86594a3cd95cf3f2e0d
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096319"
---
# <a name="certification-resource-type"></a>tipo de recurso de certificação
Namespace: microsoft.graph

Representa os detalhes de certificação de um [aplicativo](application.md). 

A propriedade de certificação de um aplicativo é somente leitura e não pode ser definida manualmente. Ele é atualizado quando o aplicativo é certificado por meio do Microsoft 365 de Conformidade do Aplicativo. Para obter mais informações, consulte [Microsoft 365 De conformidade do aplicativo](/microsoft-365-app-certification/docs/enterprise-app-certification-guide).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|certificationDetailsUrl|Cadeia de caracteres|URL que mostra detalhes de certificação para o aplicativo.|
|certificationExpirationDateTime|DateTimeOffset|O carimbo de data/hora quando a certificação atual do aplicativo expirará.|
|isCertifiedByMicrosoft|Booliano|Indica se o aplicativo é certificado pela Microsoft.|
|isPublisherAttested|Booliano|Indica se o aplicativo foi autotestado pelo desenvolvedor do aplicativo ou pelo editor.|
|lastCertificationDateTime|DateTimeOffset|O carimbo de data/hora em que a certificação do aplicativo foi adicionada ou atualizada mais recentemente.|

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
