---
title: Tipo de recurso userExperienceAnalyticsRemoteConnection
description: A experiência do usuário analisará a entidade de conexão remota.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 62d6d012e94a0423b3951d1345704d4447b81e1f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59020347"
---
# <a name="userexperienceanalyticsremoteconnection-resource-type"></a>Tipo de recurso userExperienceAnalyticsRemoteConnection

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A experiência do usuário analisará a entidade de conexão remota.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsRemoteConnections](../api/intune-devices-userexperienceanalyticsremoteconnection-list.md)|[Coleção userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)|Listar propriedades e relações dos [objetos userExperienceAnalyticsRemoteConnection.](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)|
|[Obter userExperienceAnalyticsRemoteConnection](../api/intune-devices-userexperienceanalyticsremoteconnection-get.md)|[userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)|Leia propriedades e relações do [objeto userExperienceAnalyticsRemoteConnection.](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)|
|[Criar userExperienceAnalyticsRemoteConnection](../api/intune-devices-userexperienceanalyticsremoteconnection-create.md)|[userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)|Crie um novo [objeto userExperienceAnalyticsRemoteConnection.](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)|
|[Excluir userExperienceAnalyticsRemoteConnection](../api/intune-devices-userexperienceanalyticsremoteconnection-delete.md)|Nenhum|Exclui um [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md).|
|[Atualizar userExperienceAnalyticsRemoteConnection](../api/intune-devices-userexperienceanalyticsremoteconnection-update.md)|[userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsRemoteConnection.](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)|
|[função summarizeDeviceRemoteConnection](../api/intune-devices-userexperienceanalyticsremoteconnection-summarizedeviceremoteconnection.md)|[Coleção userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo da entidade de conexão remota de análise de experiência do usuário.|
|deviceId|Cadeia de caracteres|A id do dispositivo.|
|deviceName|String|O nome do dispositivo.|
|modelo|String|O modelo de dispositivo de análise de experiência do usuário.|
|virtualNetwork|Cadeia de caracteres|A rede virtual de análise de experiência do usuário.|
|fabricante|String|O fabricante de análise de experiência do usuário.|
|deviceCount|Int32|A contagem de conexão remota. Valores válidos de 0 a 2147483647|
|cloudPcRoundTripTime|Duplo|O tempo de dica de ida e volta do dispositivo cloud pc. Valores válidos de 0 a 1,79769313486232E+308|
|cloudPcSignInTime|Duplo|A hora de entrada do dispositivo cloud pc. Valores válidos de 0 a 1,79769313486232E+308|
|remoteSignInTime|Duplo|A hora de entrada remota do dispositivo cloud pc. Valores válidos de 0 a 1,79769313486232E+308|
|coreBootTime|Duplo|O tempo de inicialização principal do Dispositivo cloud pc. Valores válidos de 0 a 1,79769313486232E+308|
|coreSignInTime|Duplo|A hora de entrada principal do dispositivo cloud pc. Valores válidos de 0 a 1,79769313486232E+308|
|cloudPcFailurePercentage|Duplo|A porcentagem de falha de entrada do dispositivo cloud pc. Valores válidos de 0 a 100|
|userPrincipalName|Cadeia de caracteres|O usuário de análise de experiência do usuárioPrincipalName.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsRemoteConnection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRemoteConnection",
  "id": "String (identifier)",
  "deviceId": "String",
  "deviceName": "String",
  "model": "String",
  "virtualNetwork": "String",
  "manufacturer": "String",
  "deviceCount": 1024,
  "cloudPcRoundTripTime": "4.2",
  "cloudPcSignInTime": "4.2",
  "remoteSignInTime": "4.2",
  "coreBootTime": "4.2",
  "coreSignInTime": "4.2",
  "cloudPcFailurePercentage": "4.2",
  "userPrincipalName": "String"
}
```



