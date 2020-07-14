---
title: tipo de recurso managedAllDeviceCertificateState
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0684e9cd6e3ca4e34c74ec6315818d94cce208fd
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124048"
---
# <a name="managedalldevicecertificatestate-resource-type"></a>tipo de recurso managedAllDeviceCertificateState

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedAllDeviceCertificateStates](../api/intune-deviceconfig-managedalldevicecertificatestate-list.md)|coleção [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|Listar Propriedades e relações dos objetos [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .|
|[Obter managedAllDeviceCertificateState](../api/intune-deviceconfig-managedalldevicecertificatestate-get.md)|[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|Leia as propriedades e as relações do objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .|
|[Criar managedAllDeviceCertificateState](../api/intune-deviceconfig-managedalldevicecertificatestate-create.md)|[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|Criar um novo objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .|
|[Excluir managedAllDeviceCertificateState](../api/intune-deviceconfig-managedalldevicecertificatestate-delete.md)|Nenhum|Exclui [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).|
|[Atualizar managedAllDeviceCertificateState](../api/intune-deviceconfig-managedalldevicecertificatestate-update.md)|[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|Atualiza as propriedades de um objeto [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|certificateRevokeStatus|[certificateRevocationStatus](../resources/intune-deviceconfig-certificaterevocationstatus.md)|Revogar status. Os valores possíveis são: `none`, `pending`, `issued`, `failed`, `revoked`.|
|certificateRevokeStatusLastChangeDateTime|DateTimeOffset|A hora em que o status da revogação foi alterado pela última vez|
|managedDeviceDisplayName|Cadeia de caracteres|Nome de exibição do dispositivo|
|userPrincipalName|Cadeia de caracteres|Nome UPN|
|certificateExpirationDateTime|DateTimeOffset|Data de vencimento do certificado|
|certificateIssuerName|Cadeia de caracteres|Emissor|
|certificateThumbprint|Cadeia de caracteres|Identificação|
|certificateSerialNumber|Cadeia de caracteres|Número de série|
|certificateSubjectName|Cadeia de caracteres|Nome do assunto do certificado|
|certificateKeyUsages|Int32|Uso de chave|
|certificateExtendedKeyUsages|Cadeia de caracteres|Uso avançado de chave|
|certificateIssuanceDateTime|DateTimeOffset|Data de emissão|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAllDeviceCertificateState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAllDeviceCertificateState",
  "id": "String (identifier)",
  "certificateRevokeStatus": "String",
  "certificateRevokeStatusLastChangeDateTime": "String (timestamp)",
  "managedDeviceDisplayName": "String",
  "userPrincipalName": "String",
  "certificateExpirationDateTime": "String (timestamp)",
  "certificateIssuerName": "String",
  "certificateThumbprint": "String",
  "certificateSerialNumber": "String",
  "certificateSubjectName": "String",
  "certificateKeyUsages": 1024,
  "certificateExtendedKeyUsages": "String",
  "certificateIssuanceDateTime": "String (timestamp)"
}
```



