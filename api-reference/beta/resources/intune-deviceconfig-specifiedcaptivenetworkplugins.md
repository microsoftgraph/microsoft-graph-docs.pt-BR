---
title: tipo de recurso specifiedCaptiveNetworkPlugins
description: Especifica todos os plug-ins de rede cativos permitidos durante a conexão VPN AlwaysOn IKEv2
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0843c5a6cc6bc71eb10c8a42f0b9ad0ac49cb328
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58785140"
---
# <a name="specifiedcaptivenetworkplugins-resource-type"></a>tipo de recurso specifiedCaptiveNetworkPlugins

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Especifica todos os plug-ins de rede cativos permitidos durante a conexão VPN AlwaysOn IKEv2

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedBundleIdentifiers|Coleção de cadeias de caracteres|Endereço do servidor IKEv2. Deve ser um FQDN, UserFQDN, endereço de rede ou ASN1DN|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.specifiedCaptiveNetworkPlugins"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.specifiedCaptiveNetworkPlugins",
  "allowedBundleIdentifiers": [
    "String"
  ]
}
```



