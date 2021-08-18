---
title: Tipo de recurso onPremEncryptedPayload
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 36fac869b01804105397e45e2840bf7eb0bf38e3b0b968bc49efa8a89ddeaf10
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54164129"
---
# <a name="onpremencryptedpayload-resource-type"></a>Tipo de recurso onPremEncryptedPayload

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar onPremEncryptedPayloads](../api/intune-raimportcerts-onpremencryptedpayload-list.md)|[Coleção onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md)|Listar propriedades e relações dos [objetos onPremEncryptedPayload.](../resources/intune-raimportcerts-onpremencryptedpayload.md)|
|[Obter onPremEncryptedPayload](../api/intune-raimportcerts-onpremencryptedpayload-get.md)|[onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md)|Ler propriedades e relações do [objeto onPremEncryptedPayload.](../resources/intune-raimportcerts-onpremencryptedpayload.md)|
|[Criar onPremEncryptedPayload](../api/intune-raimportcerts-onpremencryptedpayload-create.md)|[onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md)|Crie um novo [objeto onPremEncryptedPayload.](../resources/intune-raimportcerts-onpremencryptedpayload.md)|
|[Excluir onPremEncryptedPayload](../api/intune-raimportcerts-onpremencryptedpayload-delete.md)|Nenhum|Exclui um [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md).|
|[Atualizar onPremEncryptedPayload](../api/intune-raimportcerts-onpremencryptedpayload-update.md)|[onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md)|Atualize as propriedades de [um objeto onPremEncryptedPayload.](../resources/intune-raimportcerts-onpremencryptedpayload.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|tenantId|Guid|Ainda não documentado|
|userId|Guid|Ainda não documentado|
|deviceId|Guid|Ainda não documentado|
|payloadId|Guid|Ainda não documentado|
|deviceKeyThumbprint|String|Ainda não documentado|
|cert1PayloadUUID|String|Ainda não documentado|
|cert2PayloadUUID|String|Ainda não documentado|
|cert3PayloadUUID|String|Ainda não documentado|
|plistTemplate|String|Ainda não documentado|
|encryptedBlob|Binário|Ainda não documentado|
|payloadVersion|Int32|Ainda não documentado|
|status|Int32|Ainda não documentado|
|createdTime|DateTimeOffset|Ainda não documentado|
|lastModifiedTime|DateTimeOffset|Ainda não documentado|
|eTag|String|Ainda não documentado|
|isDeleted|Booliano|Ainda não documentado|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onPremEncryptedPayload"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onPremEncryptedPayload",
  "tenantId": "Guid",
  "userId": "Guid",
  "deviceId": "Guid",
  "payloadId": "Guid",
  "deviceKeyThumbprint": "String",
  "cert1PayloadUUID": "String",
  "cert2PayloadUUID": "String",
  "cert3PayloadUUID": "String",
  "plistTemplate": "String",
  "encryptedBlob": "binary",
  "payloadVersion": 1024,
  "status": 1024,
  "createdTime": "String (timestamp)",
  "lastModifiedTime": "String (timestamp)",
  "eTag": "String",
  "isDeleted": true
}
```




