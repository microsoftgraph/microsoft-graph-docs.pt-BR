---
title: tipo de recurso cryptographySuite
description: Parâmetros de associação de segurança vpn
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5507b36ca4ff830ecee2237be5e538eb4e00270d
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58262755"
---
# <a name="cryptographysuite-resource-type"></a>tipo de recurso cryptographySuite

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Parâmetros de associação de segurança vpn

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|encryptionMethod|[vpnEncryptionAlgorithmType](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|Método Encryption. Os valores possíveis são: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`, `chaCha20Poly1305`.|
|integrityCheckMethod|[vpnIntegrityAlgorithmType](../resources/intune-deviceconfig-vpnintegrityalgorithmtype.md)|Método de verificação de integridade. Os possíveis valores são: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`, `md5`.|
|dhGroup|[diffieHellmanGroup](../resources/intune-deviceconfig-diffiehellmangroup.md)|Grupo Diffie Hellman. Os possíveis valores são: `group1`, `group2`, `group14`, `ecp256`, `ecp384`, `group24`.|
|cipherTransformConstants|[vpnEncryptionAlgorithmType](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|Constantes de transformação de criptografia. Os valores possíveis são: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`, `chaCha20Poly1305`.|
|authenticationTransformConstants|[authenticationTransformConstant](../resources/intune-deviceconfig-authenticationtransformconstant.md)|Constantes de Transformação de Autenticação. Os possíveis valores são: `md5_96`, `sha1_96`, `sha_256_128`, `aes128Gcm`, `aes192Gcm`, `aes256Gcm`.|
|pfsGroup|[perfectForwardSecrecyGroup](../resources/intune-deviceconfig-perfectforwardsecrecygroup.md)|Grupo de Segredo de Encaminhamento Perfeito. Os valores possíveis são: `pfs1`, `pfs2`, `pfs2048`, `ecp256`, `ecp384`, `pfsMM`, `pfs24`.|

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




