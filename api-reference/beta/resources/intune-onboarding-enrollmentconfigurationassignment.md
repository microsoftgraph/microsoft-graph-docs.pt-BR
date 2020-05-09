---
title: Tipo de recurso enrollmentConfigurationAssignment
description: Atribuição de configuração de registro
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 391d618e71d337d5a3c590799239ba4c4f14e107
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178791"
---
# <a name="enrollmentconfigurationassignment-resource-type"></a>Tipo de recurso enrollmentConfigurationAssignment

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atribuição de configuração de registro

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar enrollmentConfigurationAssignments](../api/intune-onboarding-enrollmentconfigurationassignment-list.md)|Conjunto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|Listar propriedades e relações de objetos de [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).|
|[Obter enrollmentConfigurationAssignment](../api/intune-onboarding-enrollmentconfigurationassignment-get.md)|[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|Ler propriedades e relações de objetos de [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).|
|[Criar enrollmentConfigurationAssignment](../api/intune-onboarding-enrollmentconfigurationassignment-create.md)|[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|Criar um novo objeto de [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).|
|[Excluir enrollmentConfigurationAssignment](../api/intune-onboarding-enrollmentconfigurationassignment-delete.md)|Nenhum|Excluir [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).|
|[Atualizar enrollmentConfigurationAssignment](../api/intune-onboarding-enrollmentconfigurationassignment-update.md)|[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|Atualizar as propriedades de um objeto de [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da atribuição de configuração de registro|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Representa uma atribuição para dispositivos gerenciados no locatário|
|source|[deviceAndAppManagementAssignmentSource](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|Tipo de recurso usado para implantação em um grupo, direto ou policyset. Os valores possíveis são: `direct` e `policySets`.|
|sourceId|Cadeia de Caracteres|Identificador para o recurso usado para implantação em um grupo|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  },
  "source": "String",
  "sourceId": "String"
}
```



