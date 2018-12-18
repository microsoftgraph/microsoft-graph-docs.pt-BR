---
title: tipo de recurso de excludedApps
description: Contém propriedades para aplicativos de Office365 excluídos.
author: tfitzmac
ms.openlocfilehash: b8c9eff985783c953ff099dbf4d5ba00826652c4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344622"
---
# <a name="excludedapps-resource-type"></a>tipo de recurso de excludedApps

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Contém propriedades para aplicativos de Office365 excluídos.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|acesso|Boolean|O valor para se MS Office Access devem ser excluídos ou não.|
|do Excel|Boolean|O valor para se MS Office Excel devem ser excluído ou não.|
|Groove|Boolean|O valor se OneDrive do MS Office para negócios - Groove devem ser excluído ou não.|
|infoPath|Boolean|O valor para se MS Office InfoPath devem ser excluído ou não.|
|Lync|Boolean|O valor para se Skype do MS Office para negócios - Lync devem ser excluído ou não.|
|oneDrive|Boolean|O valor para se MS Office OneDrive devem ser excluído ou não.|
|oneNote|Boolean|O valor para se MS Office OneNote devem ser excluído ou não.|
|Outlook|Boolean|O valor para se MS Office Outlook devem ser excluído ou não.|
|powerPoint|Boolean|O valor para se MS Office PowerPoint devem ser excluído ou não.|
|publisher|Boolean|O valor para se MS Office Publisher devem ser excluído ou não.|
|SharePoint Designer|Boolean|O valor para se SharePoint Designer do MS Office devem ser excluído ou não.|
|Visio|Boolean|O valor para se MS Office Visio devem ser excluído ou não.|
|Word|Boolean|O valor para se MS Office Word devem ser excluído ou não.|

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





