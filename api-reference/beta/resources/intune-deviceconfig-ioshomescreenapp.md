---
title: Tipo de recurso iosHomeScreenApp
description: Representa um ícone de um aplicativo na tela inicial
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2cdaf6c263b041547056f8f6bd82e21ca880ebaa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949168"
---
# <a name="ioshomescreenapp-resource-type"></a>Tipo de recurso iosHomeScreenApp

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Representa um ícone de um aplicativo na tela inicial

Herda de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)|
|bundleID|Cadeia de caracteres|BundleID do aplicativo|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenApp",
  "displayName": "String",
  "bundleID": "String"
}
```





