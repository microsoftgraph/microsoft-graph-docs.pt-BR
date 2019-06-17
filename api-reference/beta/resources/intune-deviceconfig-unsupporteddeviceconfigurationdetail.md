---
title: tipo de recurso unsupportedDeviceConfigurationDetail
description: Uma descrição do motivo pelo qual uma entidade não é suportada.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ce838f73c4ad02ecb29d540a9f0d4af065796993
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34978966"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a>tipo de recurso unsupportedDeviceConfigurationDetail

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma descrição do motivo pelo qual uma entidade não é suportada.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|mensagem|String|Uma mensagem explicando por que uma entidade não é suportada.|
|NomeDaPropriedade|String|Se a mensagem estiver relacionada a uma propriedade específica na entidade original, o nome dessa propriedade.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfigurationDetail",
  "message": "String",
  "propertyName": "String"
}
```





