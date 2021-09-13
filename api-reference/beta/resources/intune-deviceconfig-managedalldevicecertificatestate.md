---
title: Tipo de recurso managedAllDeviceCertificateState
description: Ainda não documentado
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 84ef0315f30bb249a393b3994524ea87acca5bab
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59075476"
---
# <a name="managedalldevicecertificatestate-resource-type"></a>Tipo de recurso managedAllDeviceCertificateState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedAllDeviceCertificateStates](../api/intune-deviceconfig-managedalldevicecertificatestate-list.md)|[coleção managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|Listar propriedades e relações dos [objetos managedAllDeviceCertificateState.](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|
|[Obter managedAllDeviceCertificateState](../api/intune-deviceconfig-managedalldevicecertificatestate-get.md)|[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|Leia propriedades e relações do [objeto managedAllDeviceCertificateState.](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|
|[Criar managedAllDeviceCertificateState](../api/intune-deviceconfig-managedalldevicecertificatestate-create.md)|[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|Crie um novo [objeto managedAllDeviceCertificateState.](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|
|[Excluir managedAllDeviceCertificateState](../api/intune-deviceconfig-managedalldevicecertificatestate-delete.md)|Nenhum|Exclui [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).|
|[Atualizar managedAllDeviceCertificateState](../api/intune-deviceconfig-managedalldevicecertificatestate-update.md)|[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|Atualize as propriedades de [um objeto managedAllDeviceCertificateState.](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|certificateRevokeStatus|[certificateRevocationStatus](../resources/intune-deviceconfig-certificaterevocationstatus.md)|Revogar status. Os valores possíveis são: `none`, `pending`, `issued`, `failed`, `revoked`.|
|certificateRevokeStatusLastChangeDateTime|DateTimeOffset|A hora em que o status de revogação foi alterado pela última vez|
|managedDeviceDisplayName|String|Nome de exibição do dispositivo|
|userPrincipalName|Cadeia de caracteres|Nome UPN|
|certificateExpirationDateTime|DateTimeOffset|Data de expiração do certificado|
|certificateIssuerName|Cadeia de Caracteres|Emissor|
|certificateThumbprint|Cadeia de caracteres|Impressão Digital|
|certificateSerialNumber|String|Número de série|
|certificateSubjectName|Cadeia de Caracteres|Nome do assunto do certificado|
|certificateKeyUsages|Int32|Uso da Chave|
|certificateExtendedKeyUsages|String|Uso avançado de chave|
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



