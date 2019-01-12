---
title: tipo de recurso de excludedApps
description: Contém propriedades para aplicativos de Office365 excluídos.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 90216c639d36a989b2fad5dbdc1adbd11fe46ede
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943946"
---
# <a name="excludedapps-resource-type"></a>tipo de recurso de excludedApps

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Contém propriedades para aplicativos de Office365 excluídos.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|acesso|Booliano|O valor para se MS Office Access devem ser excluídos ou não.|
|do Excel|Booliano|O valor para se MS Office Excel devem ser excluído ou não.|
|Groove|Booliano|O valor se OneDrive do MS Office para negócios - Groove devem ser excluído ou não.|
|infoPath|Booliano|O valor para se MS Office InfoPath devem ser excluído ou não.|
|Lync|Booliano|O valor para se Skype do MS Office para negócios - Lync devem ser excluído ou não.|
|oneDrive|Booliano|O valor para se MS Office OneDrive devem ser excluído ou não.|
|oneNote|Booliano|O valor para se MS Office OneNote devem ser excluído ou não.|
|Outlook|Booliano|O valor para se MS Office Outlook devem ser excluído ou não.|
|powerPoint|Booliano|O valor para se MS Office PowerPoint devem ser excluído ou não.|
|publisher|Booliano|O valor para se MS Office Publisher devem ser excluído ou não.|
|SharePoint Designer|Booliano|O valor para se SharePoint Designer do MS Office devem ser excluído ou não.|
|Visio|Booliano|O valor para se MS Office Visio devem ser excluído ou não.|
|Word|Booliano|O valor para se MS Office Word devem ser excluído ou não.|

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
  "visio": true,
  "word": true
}
```





