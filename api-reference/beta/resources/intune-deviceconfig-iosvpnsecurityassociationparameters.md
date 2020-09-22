---
title: tipo de recurso iosVpnSecurityAssociationParameters
description: Parâmetros de associação de segurança VPN
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fc1bf75fffe3f4008171320a78d1a487cdd0771a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092661"
---
# <a name="iosvpnsecurityassociationparameters-resource-type"></a>tipo de recurso iosVpnSecurityAssociationParameters

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Parâmetros de associação de segurança VPN

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|securityEncryptionAlgorithm|[vpnEncryptionAlgorithmType](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|Algoritmo de criptografia. Os valores possíveis são: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`.|
|securityIntegrityAlgorithm|[vpnIntegrityAlgorithmType](../resources/intune-deviceconfig-vpnintegrityalgorithmtype.md)|Algoritmo de integridade. Os possíveis valores são: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`, `md5`.|
|securityDiffieHellmanGroup|Int32|Grupo Diffie-Hellman|
|lifetimeInMinutes|Int32|Tempo de vida (minutos)|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVpnSecurityAssociationParameters",
  "securityEncryptionAlgorithm": "String",
  "securityIntegrityAlgorithm": "String",
  "securityDiffieHellmanGroup": 1024,
  "lifetimeInMinutes": 1024
}
```






