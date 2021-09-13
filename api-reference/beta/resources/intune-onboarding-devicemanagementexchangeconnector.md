---
title: Tipo de recurso deviceManagementExchangeConnector
description: Entidade que representa uma conexão a um ambiente do Exchange.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2379d6a1797088b2acc2b35229921039235f4627
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59080902"
---
# <a name="devicemanagementexchangeconnector-resource-type"></a>Tipo de recurso deviceManagementExchangeConnector

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa uma conexão a um ambiente do Exchange.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementExchangeConnectors](../api/intune-onboarding-devicemanagementexchangeconnector-list.md)|Conjunto [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|Listar propriedades e relações de objeto de [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).|
|[Obter deviceManagementExchangeConnector](../api/intune-onboarding-devicemanagementexchangeconnector-get.md)|[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|Ler propriedades e relações de objetos de [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).|
|[Criar deviceManagementExchangeConnector](../api/intune-onboarding-devicemanagementexchangeconnector-create.md)|[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|Criar um novo objeto de [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).|
|[Excluir deviceManagementExchangeConnector](../api/intune-onboarding-devicemanagementexchangeconnector-delete.md)|Nenhum|Excluir [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).|
|[Atualizar deviceManagementExchangeConnector](../api/intune-onboarding-devicemanagementexchangeconnector-update.md)|[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|Atualizar as propriedades de um objeto de [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).|
|[ação de sincronização](../api/intune-onboarding-devicemanagementexchangeconnector-sync.md)|Nenhum|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Ainda não documentado|
|lastSyncDateTime|DateTimeOffset|Hora da última sincronização do Exchange Connector|
|status|[deviceManagementExchangeConnectorStatus](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|Exchange Status do conector. Os valores possíveis são: `none`, `connectionPending`, `connected`, `disconnected`.|
|primarySmtpAddress|Cadeia de caracteres|Endereço de email usado para configurar o serviço a serviço do Exchange Connector.|
|serverName|Cadeia de caracteres|O nome do servidor Exchange.|
|connectorServerName|Cadeia de caracteres|O nome do servidor que hospeda o Exchange Connector.|
|exchangeConnectorType|[deviceManagementExchangeConnectorType](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|O tipo de Exchange Connector configurado. Os valores possíveis são: `onPremises`, `hosted`, `serviceToService`, `dedicated`.|
|versão|Cadeia de caracteres|A versão do ExchangeConnectorAgent|
|exchangeAlias|Cadeia de caracteres|Um alias atribuído a um servidor Exchange|
|exchangeOrganization|Cadeia de caracteres|Organização do Exchange no servidor Exchange|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementExchangeConnector"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "id": "String (identifier)",
  "lastSyncDateTime": "String (timestamp)",
  "status": "String",
  "primarySmtpAddress": "String",
  "serverName": "String",
  "connectorServerName": "String",
  "exchangeConnectorType": "String",
  "version": "String",
  "exchangeAlias": "String",
  "exchangeOrganization": "String"
}
```



