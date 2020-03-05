---
title: tipo de recurso onPremEncryptedPayload
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 08d5f3102bb2c748d24235290a8f75abe8408334
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527593"
---
# <a name="onpremencryptedpayload-resource-type"></a>tipo de recurso onPremEncryptedPayload

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar onPremEncryptedPayloads](../api/intune-raimportcerts-onpremencryptedpayload-list.md)|coleção [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md)|Listar Propriedades e relações dos objetos [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) .|
|[Obter onPremEncryptedPayload](../api/intune-raimportcerts-onpremencryptedpayload-get.md)|[onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md)|Leia as propriedades e as relações do objeto [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) .|
|[Criar onPremEncryptedPayload](../api/intune-raimportcerts-onpremencryptedpayload-create.md)|[onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md)|Criar um novo objeto [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) .|
|[Excluir onPremEncryptedPayload](../api/intune-raimportcerts-onpremencryptedpayload-delete.md)|Nenhum|Exclui [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md).|
|[Atualizar onPremEncryptedPayload](../api/intune-raimportcerts-onpremencryptedpayload-update.md)|[onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md)|Atualiza as propriedades de um objeto [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) .|

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
|plisttemplate|String|Ainda não documentado|
|encryptedBlob|Binária|Ainda não documentado|
|payloadVersion|Int32|Ainda não documentado|
|status|Int32|Ainda não documentado|
|createdtime|DateTimeOffset|Ainda não documentado|
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



