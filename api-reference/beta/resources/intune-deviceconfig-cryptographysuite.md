---
title: tipo de recurso cryptographySuite
description: Parâmetros de associação de segurança VPN
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 26784db84c461566fa8e2d5c9d6b649fc4bfc9b8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49256810"
---
# <a name="cryptographysuite-resource-type"></a>tipo de recurso cryptographySuite

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Parâmetros de associação de segurança VPN

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|encryptionMethod|[vpnEncryptionAlgorithmType](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|Método de criptografia. Os valores possíveis são: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`.|
|integrityCheckMethod|[vpnIntegrityAlgorithmType](../resources/intune-deviceconfig-vpnintegrityalgorithmtype.md)|Método de verificação de integridade. Os possíveis valores são: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`, `md5`.|
|dhGroup|[diffieHellmanGroup](../resources/intune-deviceconfig-diffiehellmangroup.md)|Grupo Diffie Hellman. Os possíveis valores são: `group1`, `group2`, `group14`, `ecp256`, `ecp384`, `group24`.|
|cipherTransformConstants|[vpnEncryptionAlgorithmType](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|Constantes de transformação de codificação. Os valores possíveis são: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`.|
|authenticationTransformConstants|[authenticationTransformConstant](../resources/intune-deviceconfig-authenticationtransformconstant.md)|Constantes de transformação de autenticação. Os possíveis valores são: `md5_96`, `sha1_96`, `sha_256_128`, `aes128Gcm`, `aes192Gcm`, `aes256Gcm`.|
|pfsGroup|[perfectForwardSecrecyGroup](../resources/intune-deviceconfig-perfectforwardsecrecygroup.md)|Grupo de sigilo total no futuro. Os valores possíveis são: `pfs1`, `pfs2`, `pfs2048`, `ecp256`, `ecp384`, `pfsMM`, `pfs24`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cryptographySuite"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cryptographySuite",
  "encryptionMethod": "String",
  "integrityCheckMethod": "String",
  "dhGroup": "String",
  "cipherTransformConstants": "String",
  "authenticationTransformConstants": "String",
  "pfsGroup": "String"
}
```




