---
title: Tipo de recurso excludedApps
description: Contém propriedades para Aplicativos do Office365 excluídos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 45051f7526ba6d7740144e42001db28eb0443c877c4363479dcdd1a476de8bd4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54153332"
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
|bing|Boolean|O valor para se Pesquisa da Microsoft padrão deve ser excluído ou não.|
|excel|Boolean|O valor para se o MS Office Excel deve ser excluído ou não.|
|groove|Boolean|O valor para se MS Office OneDrive for Business - Groove deve ser excluído ou não.|
|infoPath|Boolean|O valor para se o MS Office InfoPath deve ser excluído ou não.|
|lync|Boolean|O valor para se MS Office Skype for Business - Lync deve ser excluído ou não.|
|oneDrive|Boolean|O valor para se o MS Office OneDrive deve ser excluído ou não.|
|oneNote|Boolean|O valor para se o MS Office OneNote deve ser excluído ou não.|
|outlook|Boolean|O valor para se o MS Office Outlook deve ser excluído ou não.|
|powerPoint|Boolean|O valor para se o MS Office PowerPoint deve ser excluído ou não.|
|publicador|Boolean|O valor para se o MS Office Publisher deve ser excluído ou não.|
|sharePointDesigner|Boolean|O valor para se MS Office SharePointDesigner deve ser excluído ou não.|
|teams|Boolean|O valor para se o MS Office Teams deve ser excluído ou não.|
|visio|Boolean|O valor para se o MS Office Visio deve ser excluído ou não.|
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




