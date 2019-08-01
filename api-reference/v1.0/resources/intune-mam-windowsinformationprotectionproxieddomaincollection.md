---
title: Tipo de recurso windowsInformationProtectionProxiedDomainCollection
description: Coleção de domínios como proxy da Proteção de Informações do Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0de9ee342cdb0fb42460d9118c87ed7e2a747b55
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037629"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a>Tipo de recurso windowsInformationProtectionProxiedDomainCollection

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Coleção de domínios como proxy da Proteção de Informações do Windows

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|Nome de exibição|
|proxiedDomains|Coleção [proxiedDomain](../resources/intune-mam-proxieddomain.md)|Coleção de domínios com proxy|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
  "displayName": "String",
  "proxiedDomains": [
    {
      "@odata.type": "microsoft.graph.proxiedDomain",
      "ipAddressOrFQDN": "String",
      "proxy": "String"
    }
  ]
}
```



