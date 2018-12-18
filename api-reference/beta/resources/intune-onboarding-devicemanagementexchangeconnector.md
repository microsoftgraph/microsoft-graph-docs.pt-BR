---
title: Tipo de recurso deviceManagementExchangeConnector
description: Entidade que representa uma conexão a um ambiente do Exchange.
author: tfitzmac
ms.openlocfilehash: 726afd7957f8e95d38b68065b1bc99f884a9208d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312023"
---
# <a name="devicemanagementexchangeconnector-resource-type"></a>Tipo de recurso deviceManagementExchangeConnector

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

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
|id|String|Ainda não documentado|
|lastSyncDateTime|DateTimeOffset|Hora da última sincronização do Exchange Connector|
|status|[deviceManagementExchangeConnectorStatus](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|Status de conector do Exchange. Os valores possíveis são: `none`, `connectionPending`, `connected`, `disconnected`.|
|primarySmtpAddress|Cadeia de caracteres|Endereço de email usado para configurar o serviço a serviço do Exchange Connector.|
|serverName|Cadeia de caracteres|O nome do servidor do Exchange.|
|connectorServerName|Cadeia de caracteres|O nome do servidor que hospeda o Exchange Connector.|
|exchangeConnectorType|[deviceManagementExchangeConnectorType](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|O tipo de Exchange Connector configurado. Os valores possíveis são: `onPremises`, `hosted`, `serviceToService`, `dedicated`.|
|version|Cadeia de caracteres|A versão do ExchangeConnectorAgent|
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





