---
title: Tipo de recurso reportRoot
description: O recurso que representa uma instância de um dispositivo ou relatório de solução de problemas, dependendo do contexto.
ms.localizationpriority: medium
author: rolyon
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 56e3bc6d11c913a35ee69a803a7e038a86971518
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59115272"
---
# <a name="reportroot-resource-type"></a>Tipo de recurso reportRoot

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

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
|[Função managedDeviceEnrollmentAbandonmentDetails](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[relatório](../resources/intune-shared-report.md)|Relatório de detalhes de abandono de registro de metadados|
|[Função managedDeviceEnrollmentAbandonmentSummary](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[relatório](../resources/intune-shared-report.md)|Metadados para relatório de resumo de abandono de registro|
|[Função managedDeviceEnrollmentFailureDetails](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|Ainda não documentado|
|[Função managedDeviceEnrollmentFailureTrends](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|Metadados para o relatório de tendências de falha de registro|
|[Função managedDeviceEnrollmentTopFailures](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|Ainda não documentado|

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



