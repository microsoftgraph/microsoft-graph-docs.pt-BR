---
title: Tipo de recurso userExperienceAnalyticsDeviceStartupProcess
description: Os detalhes do processo de inicialização do dispositivo de análise de experiência do usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f79e36f7eabf1d39aab7563b21cc5b2da5bffe5240b70d1f371ca26c4b8e6cf5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54224597"
---
# <a name="userexperienceanalyticsdevicestartupprocess-resource-type"></a>Tipo de recurso userExperienceAnalyticsDeviceStartupProcess

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Os detalhes do processo de inicialização do dispositivo de análise de experiência do usuário.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsDeviceStartupProcesses](../api/intune-devices-userexperienceanalyticsdevicestartupprocess-list.md)|[Coleção userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)|Listar propriedades e relações dos [objetos userExperienceAnalyticsDeviceStartupProcess.](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)|
|[Obter userExperienceAnalyticsDeviceStartupProcess](../api/intune-devices-userexperienceanalyticsdevicestartupprocess-get.md)|[userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)|Leia propriedades e relações do [objeto userExperienceAnalyticsDeviceStartupProcess.](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)|
|[Criar userExperienceAnalyticsDeviceStartupProcess](../api/intune-devices-userexperienceanalyticsdevicestartupprocess-create.md)|[userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)|Crie um novo [objeto userExperienceAnalyticsDeviceStartupProcess.](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)|
|[Excluir userExperienceAnalyticsDeviceStartupProcess](../api/intune-devices-userexperienceanalyticsdevicestartupprocess-delete.md)|Nenhum|Exclui um [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md).|
|[Atualizar userExperienceAnalyticsDeviceStartupProcess](../api/intune-devices-userexperienceanalyticsdevicestartupprocess-update.md)|[userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsDeviceStartupProcess.](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do processo de inicialização do dispositivo de análise de experiência do usuário.|
|managedDeviceId|Cadeia de caracteres|A ID do dispositivo de análise de experiência do usuário.|
|processName|Cadeia de caracteres|Nome do processo de inicialização do dispositivo de análise de experiência do usuário.|
|productName|Cadeia de caracteres|O nome do produto do processo de inicialização do dispositivo de análise de experiência do usuário.|
|publicador|String|O editor de processo de inicialização do dispositivo de análise de experiência do usuário.|
|startupImpactInMs|Int32|Impacto no processo de inicialização do dispositivo de análise de experiência do usuário em milissegundos.|

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




