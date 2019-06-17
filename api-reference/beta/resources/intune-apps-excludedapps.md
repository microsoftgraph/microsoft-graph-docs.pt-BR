---
title: tipo de recurso excludedApps
description: Contém propriedades para aplicativos do Office365 excluídos.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 91418a1a60a87f381dc15c63a60d69e8c264a5c3
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991244"
---
# <a name="excludedapps-resource-type"></a>tipo de recurso excludedApps

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para aplicativos do Office365 excluídos.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Access|Booliano|O valor de se o MS Office Access deve ser excluído ou não.|
|Ele|Booliano|O valor de se o MS Office Excel deve ser excluído ou não.|
|Groove|Booliano|O valor de se o MS Office OneDrive for Business-Groove deve ser excluído ou não.|
|Destina|Booliano|O valor de se o MS Office InfoPath deve ou não ser excluído.|
|Lync|Booliano|O valor de se o MS Office Skype for Business-Lync deve ser excluído ou não.|
|oneDrive|Booliano|O valor de se o MS Office OneDrive deve ser excluído ou não.|
|oneNote|Booliano|O valor de se o MS Office OneNote deve ser excluído ou não.|
|outlook|Booliano|O valor de se o MS Office Outlook deve ser excluído ou não.|
|Apresentação|Booliano|O valor de se o MS Office PowerPoint deve ser excluído ou não.|
|publicador|Booliano|O valor de se o MS Office Publisher deve ser excluído ou não.|
|sharePointDesigner|Booliano|O valor de se o MS Office SharePointDesigner deve ser excluído ou não.|
|Teams|Booliano|O valor de se as equipes do MS Office devem ser excluídas ou não.|
|Visio|Booliano|O valor de se o MS Office Visio deve ser excluído ou não.|
|palavras|Booliano|O valor de se o MS Office Word deve ser excluído ou não.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.excludedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.excludedApps",
  "access": true,
  "excel": true,
  "groove": true,
  "infoPath": true,
  "lync": true,
  "oneDrive": true,
  "oneNote": true,
  "outlook": true,
  "powerPoint": true,
  "publisher": true,
  "sharePointDesigner": true,
  "teams": true,
  "visio": true,
  "word": true
}
```





