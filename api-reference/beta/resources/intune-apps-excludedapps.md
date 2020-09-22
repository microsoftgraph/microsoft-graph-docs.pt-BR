---
title: tipo de recurso excludedApps
description: Contém propriedades para aplicativos do Office365 excluídos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 30aaecee77c4cdea7539e790fd1204ecd9e8dc98
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003931"
---
# <a name="excludedapps-resource-type"></a>tipo de recurso excludedApps

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para aplicativos do Office365 excluídos.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Access|Boolean|O valor de se o MS Office Access deve ser excluído ou não.|
|Bing|Boolean|O valor da pesquisa da Microsoft como padrão deve ser excluído ou não.|
|Ele|Boolean|O valor de se o MS Office Excel deve ser excluído ou não.|
|Groove|Boolean|O valor de se o MS Office OneDrive for Business-Groove deve ser excluído ou não.|
|Destina|Boolean|O valor de se o MS Office InfoPath deve ou não ser excluído.|
|Lync|Boolean|O valor de se o MS Office Skype for Business-Lync deve ser excluído ou não.|
|oneDrive|Boolean|O valor de se o MS Office OneDrive deve ser excluído ou não.|
|oneNote|Boolean|O valor de se o MS Office OneNote deve ser excluído ou não.|
|outlook|Boolean|O valor de se o MS Office Outlook deve ser excluído ou não.|
|Apresentação|Boolean|O valor de se o MS Office PowerPoint deve ser excluído ou não.|
|publicador|Boolean|O valor de se o MS Office Publisher deve ser excluído ou não.|
|sharePointDesigner|Boolean|O valor de se o MS Office SharePointDesigner deve ser excluído ou não.|
|Teams|Boolean|O valor de se as equipes do MS Office devem ser excluídas ou não.|
|Visio|Boolean|O valor de se o MS Office Visio deve ser excluído ou não.|
|palavras|Boolean|O valor de se o MS Office Word deve ser excluído ou não.|

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
  "bing": true,
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






