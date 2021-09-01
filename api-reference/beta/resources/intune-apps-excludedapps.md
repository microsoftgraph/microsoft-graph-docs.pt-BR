---
title: Tipo de recurso excludedApps
description: Contém propriedades para Aplicativos do Office365 excluídos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1ac91ac42018c5fc687a0b89d7496c1fdc15c97d
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58783593"
---
# <a name="excludedapps-resource-type"></a>Tipo de recurso excludedApps

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para Aplicativos do Office365 excluídos.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|access|Boleano|O valor para se o MS Office Access deve ser excluído ou não.|
|bing|Boleano|O valor para se Pesquisa da Microsoft padrão deve ser excluído ou não.|
|excel|Boleano|O valor para se o MS Office Excel deve ser excluído ou não.|
|groove|Boleano|O valor para se MS Office OneDrive for Business - Groove deve ser excluído ou não.|
|infoPath|Boleano|O valor para se o MS Office InfoPath deve ser excluído ou não.|
|lync|Boleano|O valor para se MS Office Skype for Business - Lync deve ser excluído ou não.|
|oneDrive|Booliano|O valor para se o MS Office OneDrive deve ser excluído ou não.|
|oneNote|Boleano|O valor para se o MS Office OneNote deve ser excluído ou não.|
|outlook|Boleano|O valor para se o MS Office Outlook deve ser excluído ou não.|
|powerPoint|Boleano|O valor para se o MS Office PowerPoint deve ser excluído ou não.|
|publicador|Boleano|O valor para se o MS Office Publisher deve ser excluído ou não.|
|sharePointDesigner|Boleano|O valor para se MS Office SharePointDesigner deve ser excluído ou não.|
|teams|Boleano|O valor para se o MS Office Teams deve ser excluído ou não.|
|visio|Boleano|O valor para se o MS Office Visio deve ser excluído ou não.|
|word|Booliano|O valor para se o MS Office Word deve ser excluído ou não.|

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



