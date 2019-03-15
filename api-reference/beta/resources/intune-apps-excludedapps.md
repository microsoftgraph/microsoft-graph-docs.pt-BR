---
title: tipo de recurso excludedApps
description: Contém propriedades para aplicativos do Office365 excluídos.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8dee0d5328f1f69c95159116bf913bc2abb959d7
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571687"
---
# <a name="excludedapps-resource-type"></a>tipo de recurso excludedApps

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para aplicativos do Office365 excluídos.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Access|Boolean|O valor de se o MS Office Access deve ser excluído ou não.|
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
Nenhuma

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




