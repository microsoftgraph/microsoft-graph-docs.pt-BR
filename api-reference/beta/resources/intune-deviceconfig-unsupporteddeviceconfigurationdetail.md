---
title: tipo de recurso de unsupportedDeviceConfigurationDetail
description: Uma descrição por que não há suporte para uma entidade.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0a213961e6b816917b061bc56c792cf9a60e3a2a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839470"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a>tipo de recurso de unsupportedDeviceConfigurationDetail

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Uma descrição por que não há suporte para uma entidade.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|mensagem|String|Uma mensagem que explica por que não há suporte para uma entidade.|
|propertyName|Cadeia de caracteres|Se a mensagem está relacionada a uma propriedade específica à entidade original e, em seguida, o nome dessa propriedade.|

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





