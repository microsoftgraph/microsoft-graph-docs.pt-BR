---
title: Tipo de recurso reportRoot
description: O recurso que representa uma instância dos Relatórios de históricos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 72e4581ded72b9e22eba3fa0d10382ed1b3a5101
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60445493"
---
# <a name="reportroot-resource-type"></a>Tipo de recurso reportRoot

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso que representa uma instância dos Relatórios de históricos.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter reportRoot](../api/intune-deviceconfig-reportroot-get.md)|[reportRoot](../resources/intune-deviceconfig-reportroot.md)|Ler propriedades e relações de objetos de [reportRoot](../resources/intune-deviceconfig-reportroot.md).|
|[Atualizar reportRoot](../api/intune-deviceconfig-reportroot-update.md)|[reportRoot](../resources/intune-deviceconfig-reportroot.md)|Atualizar as propriedades de um objeto de [reportRoot](../resources/intune-deviceconfig-reportroot.md).|
|[Função deviceConfigurationUserActivity](../api/intune-deviceconfig-reportroot-deviceconfigurationuseractivity.md)|[relatório](../resources/intune-deviceconfig-report.md)|Metadados para o Relatório de atividades do usuário de configuração do dispositivo|
|[função deviceConfigurationDeviceActivity](../api/intune-deviceconfig-reportroot-deviceconfigurationdeviceactivity.md)|[relatório](../resources/intune-deviceconfig-report.md)|Metadados para o relatório de atividade do dispositivo de configuração do dispositivo|

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



