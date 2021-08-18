---
title: Tipo de recurso complianceManagementPartner
description: Parceiro de gerenciamento de conformidade para todas as plataformas
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e4acb774a6478f2d3bfd27c582c245ecea605d092896ef89b3a746a32e67db9a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235986"
---
# <a name="compliancemanagementpartner-resource-type"></a>Tipo de recurso complianceManagementPartner

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Parceiro de gerenciamento de conformidade para todas as plataformas

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar complianceManagementPartners](../api/intune-onboarding-compliancemanagementpartner-list.md)|[coleção complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)|Listar propriedades e relações dos [objetos complianceManagementPartner.](../resources/intune-onboarding-compliancemanagementpartner.md)|
|[Obter complianceManagementPartner](../api/intune-onboarding-compliancemanagementpartner-get.md)|[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)|Ler propriedades e relações do [objeto complianceManagementPartner.](../resources/intune-onboarding-compliancemanagementpartner.md)|
|[Criar complianceManagementPartner](../api/intune-onboarding-compliancemanagementpartner-create.md)|[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)|Crie um novo [objeto complianceManagementPartner.](../resources/intune-onboarding-compliancemanagementpartner.md)|
|[Excluir complianceManagementPartner](../api/intune-onboarding-compliancemanagementpartner-delete.md)|Nenhum|Exclui um [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md).|
|[Atualizar complianceManagementPartner](../api/intune-onboarding-compliancemanagementpartner-update.md)|[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)|Atualize as propriedades de [um objeto complianceManagementPartner.](../resources/intune-onboarding-compliancemanagementpartner.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID da entidade|
|lastHeartbeatDateTime|DateTimeOffset|Timestamp de última pulsação depois que o administrador entrou no parceiro de gerenciamento de conformidade|
|partnerState|[deviceManagementPartnerTenantState](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|Estado do parceiro desse locatário. Os possíveis valores são: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.|
|displayName|Cadeia de caracteres|Nome de exibição de parceiro|
|macOsOnboarded|Boolean|Parceiro a bordo para dispositivos Mac.|
|windowsOnboarded|Boolean|Parceiro integrado para Windows dispositivos.|
|androidOnboarded|Boolean|Parceiro a bordo para dispositivos Android.|
|iosOnboarded|Boolean|Parceiro internado para dispositivos ios.|
|macOsEnrollmentAssignments|[coleção complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)|Grupos de usuários que registram dispositivos Mac por meio de parceiros.|
|windowsEnrollmentAssignments|[coleção complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)|Grupos de usuários que registram Windows por meio de parceiros.|
|androidEnrollmentAssignments|[coleção complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)|Grupos de usuários que registram dispositivos Android por meio de parceiros.|
|iosEnrollmentAssignments|[coleção complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)|Grupos de usuários que registram dispositivos ios por meio de parceiros.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.complianceManagementPartner"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.complianceManagementPartner",
  "id": "String (identifier)",
  "lastHeartbeatDateTime": "String (timestamp)",
  "partnerState": "String",
  "displayName": "String",
  "macOsOnboarded": true,
  "windowsOnboarded": true,
  "androidOnboarded": true,
  "iosOnboarded": true,
  "macOsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "String",
        "deviceAndAppManagementAssignmentFilterType": "String",
        "collectionId": "String"
      }
    }
  ],
  "windowsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "String",
        "deviceAndAppManagementAssignmentFilterType": "String",
        "collectionId": "String"
      }
    }
  ],
  "androidEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "String",
        "deviceAndAppManagementAssignmentFilterType": "String",
        "collectionId": "String"
      }
    }
  ],
  "iosEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "String",
        "deviceAndAppManagementAssignmentFilterType": "String",
        "collectionId": "String"
      }
    }
  ]
}
```




