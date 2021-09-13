---
title: Tipo de recurso excludedApps
description: Contém propriedades para Aplicativos do Office365 excluídos.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2025df58d8ff6387fb217ec2d19e7f6d34df2499
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59064564"
---
# <a name="excludedapps-resource-type"></a>Tipo de recurso excludedApps

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para Aplicativos do Office365 excluídos.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|access|Boolean|O valor para se o MS Office Access deve ser excluído ou não.|
|bing|Boleano|O valor para se Pesquisa da Microsoft padrão deve ser excluído ou não.|
|excel|Boolean|O valor para se o MS Office Excel deve ser excluído ou não.|
|groove|Booliano|O valor para se MS Office OneDrive for Business - Groove deve ser excluído ou não.|
|infoPath|Boolean|O valor para se o MS Office InfoPath deve ser excluído ou não.|
|lync|Booliano|O valor para se MS Office Skype for Business - Lync deve ser excluído ou não.|
|oneDrive|Boleano|O valor para se o MS Office OneDrive deve ser excluído ou não.|
|oneNote|Boleano|O valor para se o MS Office OneNote deve ser excluído ou não.|
|outlook|Boleano|O valor para se o MS Office Outlook deve ser excluído ou não.|
|powerPoint|Booliano|O valor para se o MS Office PowerPoint deve ser excluído ou não.|
|publicador|Boolean|O valor para se o MS Office Publisher deve ser excluído ou não.|
|sharePointDesigner|Boleano|O valor para se MS Office SharePointDesigner deve ser excluído ou não.|
|teams|Booliano|O valor para se o MS Office Teams deve ser excluído ou não.|
|visio|Booliano|O valor para se o MS Office Visio deve ser excluído ou não.|
|word|Boolean|O valor para se o MS Office Word deve ser excluído ou não.|

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



