---
title: Tipo de recurso cloudPCConnectivityIssue
description: A entidade de problema de conectividade de análise da experiência do usuário.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4f1b08cc38f0d152a1b01fb7fa972781bbe5b4aa
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59131200"
---
# <a name="cloudpcconnectivityissue-resource-type"></a>Tipo de recurso cloudPCConnectivityIssue

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de problema de conectividade de análise da experiência do usuário.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar cloudPCConnectivityIssues](../api/intune-devices-cloudpcconnectivityissue-list.md)|[Coleção cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md)|Listar propriedades e relações dos objetos [cloudPCConnectivityIssue.](../resources/intune-devices-cloudpcconnectivityissue.md)|
|[Obter cloudPCConnectivityIssue](../api/intune-devices-cloudpcconnectivityissue-get.md)|[cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md)|Leia propriedades e relações do [objeto cloudPCConnectivityIssue.](../resources/intune-devices-cloudpcconnectivityissue.md)|
|[Criar cloudPCConnectivityIssue](../api/intune-devices-cloudpcconnectivityissue-create.md)|[cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md)|Crie um novo [objeto cloudPCConnectivityIssue.](../resources/intune-devices-cloudpcconnectivityissue.md)|
|[Excluir cloudPCConnectivityIssue](../api/intune-devices-cloudpcconnectivityissue-delete.md)|Nenhum|Exclui um [cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md).|
|[Atualizar cloudPCConnectivityIssue](../api/intune-devices-cloudpcconnectivityissue-update.md)|[cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md)|Atualize as propriedades de [um objeto cloudPCConnectivityIssue.](../resources/intune-devices-cloudpcconnectivityissue.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo da entidade de evento de problema de conectividade de análise de experiência do usuário.|
|deviceId|Cadeia de caracteres|O DeviceId do Intune do dispositivo ao que a conexão está associada.|
|errorCode|Cadeia de caracteres|O código de erro do problema de conectividade.|
|errorDateTime|DateTimeOffset|A hora em que a conexão foi iniciada. O tempo é mostrado no formato ISO 8601 e hora UTC (Tempo Universal Coordenado).|
|userId|Cadeia de caracteres|A ID exclusiva do usuário que inicializa a conexão.|
|errorDescription|Cadeia de caracteres|A descrição detalhada do que deu errado.|
|recommendedAction|Cadeia de Caracteres|A ação recomendada para corrigir o erro correspondente.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPCConnectivityIssue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPCConnectivityIssue",
  "id": "String (identifier)",
  "deviceId": "String",
  "errorCode": "String",
  "errorDateTime": "String (timestamp)",
  "userId": "String",
  "errorDescription": "String",
  "recommendedAction": "String"
}
```



