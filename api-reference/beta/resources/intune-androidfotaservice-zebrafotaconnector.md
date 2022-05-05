---
title: Tipo de recurso zebraFotaConnector
description: A entidade de conector zebra FOTA que representa o status de autorização do locatário para Intune chamar o Zebra Update Services.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ae01c91dc398f2780b4f0288233664c36ad7a8b4
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213008"
---
# <a name="zebrafotaconnector-resource-type"></a>Tipo de recurso zebraFotaConnector

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de conector zebra FOTA que representa o status de autorização do locatário para Intune chamar o Zebra Update Services.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter zebraFotaConnector](../api/intune-androidfotaservice-zebrafotaconnector-get.md)|[zebraFotaConnector](../resources/intune-androidfotaservice-zebrafotaconnector.md)|Ler propriedades e relações do objeto [zebraFotaConnector](../resources/intune-androidfotaservice-zebrafotaconnector.md) .|
|[Atualizar zebraFotaConnector](../api/intune-androidfotaservice-zebrafotaconnector-update.md)|[zebraFotaConnector](../resources/intune-androidfotaservice-zebrafotaconnector.md)|Atualize as propriedades de um [objeto zebraFotaConnector](../resources/intune-androidfotaservice-zebrafotaconnector.md) .|
|[ação hasActiveDeployments](../api/intune-androidfotaservice-zebrafotaconnector-hasactivedeployments.md)|Booliano|Ainda não documentado|
|[Ação approveFotaApps](../api/intune-androidfotaservice-zebrafotaconnector-approvefotaapps.md)|Booliano|Ainda não documentado|
|[ação de conexão](../api/intune-androidfotaservice-zebrafotaconnector-connect.md)|Booliano|Ainda não documentado|
|[ação de desconectar](../api/intune-androidfotaservice-zebrafotaconnector-disconnect.md)|Booliano|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID de ZebraFotaConnector.|
|estado|[zebraFotaConnectorState](../resources/intune-androidfotaservice-zebrafotaconnectorstate.md)|O estado do conector Zebra. Os valores possíveis são: `none`, `connected`, `disconnected`, `unknownFutureValue`.|
|enrollmentToken|Cadeia de Caracteres|Token de registro de locatário da Zebra. O token é usado para registrar dispositivos Zebra no Serviço FOTA por meio da configuração do aplicativo.|
|enrollmentAuthorizationUrl|Cadeia de Caracteres|Conclua a URL de autorização de registro de conta. Isso corresponde ao verification_uri_complete nas documentações da API zebra.|
|lastSyncDateTime|DateTimeOffset|Data e hora em que a conta foi sincronizada pela última vez com a Zebra|
|fotaAppsApproved|Booliano|Sinalizador que indica se os aplicativos FOTA (Firmware Over-the-Air) necessários foram aprovados.|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.zebraFotaConnector"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.zebraFotaConnector",
  "id": "String (identifier)",
  "state": "String",
  "enrollmentToken": "String",
  "enrollmentAuthorizationUrl": "String",
  "lastSyncDateTime": "String (timestamp)",
  "fotaAppsApproved": true
}
```




