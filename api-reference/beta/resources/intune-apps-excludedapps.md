---
title: tipo de recurso de excludedApps
description: Contém propriedades para aplicativos de Office365 excluídos.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1d3cd9a159597689a64070181640415a6ce2fc61
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395675"
---
# <a name="excludedapps-resource-type"></a>tipo de recurso de excludedApps

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

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




