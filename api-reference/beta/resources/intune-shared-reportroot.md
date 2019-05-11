---
title: Tipo de recurso reportRoot
description: O recurso que representa uma instância de um dispositivo ou relatório de solução de problemas, dependendo do contexto.
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: c975abfa3cb580d107967c7adaf66627bad2ad2e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33938727"
---
# <a name="reportroot-resource-type"></a>Tipo de recurso reportRoot

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso que representa uma instância de um dispositivo ou relatório de solução de problemas, dependendo do contexto.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter reportRoot](../api/intune-shared-reportroot-get.md)|Ler propriedades e relações de objetos de [reportRoot](../resources/intune-shared-reportroot.md).|
|[Atualizar reportRoot](../api/intune-shared-reportroot-update.md)|Atualizar as propriedades de um objeto [reportRoot](../resources/intune-shared-reportroot.md).|
|**Configuração do dispositivo**|
|[Função deviceConfigurationUserActivity](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|Metadados para o Relatório de atividades do usuário de configuração do dispositivo|
|[função deviceConfigurationDeviceActivity](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|Metadados para o relatório de atividade do dispositivo de configuração do dispositivo|
|**Solução de Problemas**|
|[função managedDeviceEnrollmentAbandonmentDetails](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[relatório](../resources/intune-shared-report.md)|Metadados para o relatório de detalhes de abandono de registro|
|[função managedDeviceEnrollmentAbandonmentSummary](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[relatório](../resources/intune-shared-report.md)|Metadados para o relatório de Resumo de abandono de registro|
|[função managedDeviceEnrollmentFailureDetails](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|Ainda não documentado|
|[função managedDeviceEnrollmentFailureTrends](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|Metadados para o relatório de tendências de falha de inscrição|
|[função managedDeviceEnrollmentTopFailures](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo dessa entidade.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "String (identifier)"
}
```



