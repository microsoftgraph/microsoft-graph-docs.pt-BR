---
title: tipo de recurso iosVpnSecurityAssociationParameters
description: Parâmetros de associação de segurança VPN
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4ecf2597222a578d342f69c16c665c493b8c3329
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002725"
---
# <a name="iosvpnsecurityassociationparameters-resource-type"></a>tipo de recurso iosVpnSecurityAssociationParameters

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Parâmetros de associação de segurança VPN

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|securityEncryptionAlgorithm|[vpnEncryptionAlgorithmType](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|Algoritmo de criptografia. Os possíveis valores são: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`.|
|securityIntegrityAlgorithm|[vpnIntegrityAlgorithmType](../resources/intune-deviceconfig-vpnintegrityalgorithmtype.md)|Algoritmo de integridade. Os valores possíveis são: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`.|
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





