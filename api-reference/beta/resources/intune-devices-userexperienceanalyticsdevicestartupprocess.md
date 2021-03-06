---
title: tipo de recurso userExperienceAnalyticsDeviceStartupProcess
description: Os detalhes do processo de inicialização do dispositivo de análise da experiência do usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f92967d6cf7fe4d4be381bd2066d477b906eed1f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49208342"
---
# <a name="userexperienceanalyticsdevicestartupprocess-resource-type"></a>tipo de recurso userExperienceAnalyticsDeviceStartupProcess

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Os detalhes do processo de inicialização do dispositivo de análise da experiência do usuário.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsDeviceStartupProcesses](../api/intune-devices-userexperienceanalyticsdevicestartupprocess-list.md)|coleção [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)|Listar Propriedades e relações dos objetos [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) .|
|[Obter userExperienceAnalyticsDeviceStartupProcess](../api/intune-devices-userexperienceanalyticsdevicestartupprocess-get.md)|[userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)|Leia as propriedades e as relações do objeto [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) .|
|[Criar userExperienceAnalyticsDeviceStartupProcess](../api/intune-devices-userexperienceanalyticsdevicestartupprocess-create.md)|[userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)|Criar um novo objeto [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) .|
|[Excluir userExperienceAnalyticsDeviceStartupProcess](../api/intune-devices-userexperienceanalyticsdevicestartupprocess-delete.md)|Nenhum|Exclui [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md).|
|[Atualizar userExperienceAnalyticsDeviceStartupProcess](../api/intune-devices-userexperienceanalyticsdevicestartupprocess-update.md)|[userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)|Atualiza as propriedades de um objeto [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do processo de inicialização do dispositivo de análise da experiência do usuário.|
|managedDeviceId|String|A ID do dispositivo de análise da experiência do usuário.|
|Process|String|Nome do processo de inicialização do dispositivo de análise da experiência do usuário.|
|productName|Cadeia de caracteres|O nome do produto do processo de inicialização do dispositivo analítico da experiência do usuário.|
|publicador|String|O fornecedor da experiência do usuário do processo de inicialização do dispositivo de análise.|
|startupImpactInMs|Int32|Impacto do processo de inicialização do dispositivo de análise de experiência do usuário em milissegundos.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsDeviceStartupProcess"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcess",
  "id": "String (identifier)",
  "managedDeviceId": "String",
  "processName": "String",
  "productName": "String",
  "publisher": "String",
  "startupImpactInMs": 1024
}
```




