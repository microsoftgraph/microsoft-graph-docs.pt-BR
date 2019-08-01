---
title: Tipo de recurso reportRoot
description: O recurso que representa uma instância dos Relatórios de históricos.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8a8fa8011ad4550ec80acd0b4d6d2159f10647de
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036859"
---
# <a name="reportroot-resource-type"></a>Tipo de recurso reportRoot

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso que representa uma instância dos Relatórios de históricos.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter reportRoot](../api/intune-shared-reportroot-get.md)|[reportRoot](../resources/intune-shared-reportroot.md)|Ler propriedades e relações de objetos de [reportRoot](../resources/intune-shared-reportroot.md).|
|[Atualizar reportRoot](../api/intune-shared-reportroot-update.md)|[reportRoot](../resources/intune-shared-reportroot.md)|Atualizar as propriedades de um objeto de [reportRoot](../resources/intune-shared-reportroot.md).|
|**Configuração do dispositivo**|
|[função deviceConfigurationDeviceActivity](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|[relatório](../resources/intune-shared-report.md)|Metadados para o relatório de atividade do dispositivo de configuração do dispositivo|
|[Função deviceConfigurationUserActivity](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|[relatório](../resources/intune-shared-report.md)|Metadados para o Relatório de atividades do usuário de configuração do dispositivo|
|**Solução de Problemas**|
|[função managedDeviceEnrollmentFailureDetails](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|[relatório](../resources/intune-shared-report.md)|Ainda não documentado.|
|[função managedDeviceEnrollmentTopFailures](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|[relatório](../resources/intune-shared-report.md)|Ainda não documentado.|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo dessa entidade.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "String (identifier)"
}
```

## <a name="example"></a>Exemplo

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/reports
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.reportRoot"}-->
```json
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```
