---
title: tipo de recurso unsupportedDeviceConfigurationDetail
description: Uma descrição do motivo pelo qual uma entidade não é suportada.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0d03c25d542d598aab7df9763baa33956f9a6a01
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49276417"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a>tipo de recurso unsupportedDeviceConfigurationDetail

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma descrição do motivo pelo qual uma entidade não é suportada.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|mensagem|String|Uma mensagem explicando por que uma entidade não é suportada.|
|propertyName|String|Se a mensagem estiver relacionada a uma propriedade específica na entidade original, o nome dessa propriedade.|

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




