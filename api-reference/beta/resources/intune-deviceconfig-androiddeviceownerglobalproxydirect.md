---
title: Tipo de recurso androidDeviceOwnerGlobalProxyDirect
description: Android Device Owner Global Proxy Direct.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6f1c3e169492176e2420af46c85fbd3c596c5b77
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59148036"
---
# <a name="androiddeviceownerglobalproxydirect-resource-type"></a>Tipo de recurso androidDeviceOwnerGlobalProxyDirect

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Android Device Owner Global Proxy Direct.


Herda de [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|host|Cadeia de Caracteres|O nome do host|
|port|Int32|A porta|
|excludedHosts|String collection|Os hosts excluídos|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyDirect"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGlobalProxyDirect",
  "host": "String",
  "port": 1024,
  "excludedHosts": [
    "String"
  ]
}
```



