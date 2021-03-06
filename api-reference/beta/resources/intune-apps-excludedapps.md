---
title: tipo de recurso excludedApps
description: Contém propriedades para aplicativos do Office365 excluídos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4f4a481d52b06c59d9d79df439b41152600af989
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49274282"
---
# <a name="excludedapps-resource-type"></a>tipo de recurso excludedApps

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para aplicativos do Office365 excluídos.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Access|Booliano|O valor de se o MS Office Access deve ser excluído ou não.|
|Bing|Booliano|O valor da pesquisa da Microsoft como padrão deve ser excluído ou não.|
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




