---
title: Tipo de recurso deviceManagementReports
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de relatórios.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cbcffd77d9002477c2f20fc54f8909e60cc2c70b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086131"
---
# <a name="devicemanagementreports-resource-type"></a>Tipo de recurso deviceManagementReports

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade singleton que atua como um contêiner para todas as funcionalidades de relatórios.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceManagementReports](../api/intune-grouppolicy-devicemanagementreports-get.md)|[deviceManagementReports](../resources/intune-grouppolicy-devicemanagementreports.md)|Leia propriedades e relações do [objeto deviceManagementReports.](../resources/intune-grouppolicy-devicemanagementreports.md)|
|[Atualizar deviceManagementReports](../api/intune-grouppolicy-devicemanagementreports-update.md)|[deviceManagementReports](../resources/intune-grouppolicy-devicemanagementreports.md)|Atualize as propriedades de [um objeto deviceManagementReports.](../resources/intune-grouppolicy-devicemanagementreports.md)|
|[ação getGroupPolicySettingsDeviceSettingsReport](../api/intune-grouppolicy-devicemanagementreports-getgrouppolicysettingsdevicesettingsreport.md)|Fluxo|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo dessa entidade|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementReports"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementReports",
  "id": "String (identifier)"
}
```



