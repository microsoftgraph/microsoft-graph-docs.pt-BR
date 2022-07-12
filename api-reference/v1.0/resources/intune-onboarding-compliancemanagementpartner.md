---
title: Tipo de recurso complianceManagementPartner
description: Parceiro de gerenciamento de conformidade para todas as plataformas
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5098c5adc788ef3c807d6fd36c29986eb9ae5c01
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66735996"
---
# <a name="compliancemanagementpartner-resource-type"></a>Tipo de recurso complianceManagementPartner

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Parceiro de gerenciamento de conformidade para todas as plataformas

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar complianceManagementPartners](../api/intune-onboarding-compliancemanagementpartner-list.md)|[coleção complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)|Listar propriedades e relações dos [objetos complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) .|
|[Obter complianceManagementPartner](../api/intune-onboarding-compliancemanagementpartner-get.md)|[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)|Ler propriedades e relações do [objeto complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) .|
|[Criar complianceManagementPartner](../api/intune-onboarding-compliancemanagementpartner-create.md)|[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)|Crie um novo [objeto complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) .|
|[Excluir complianceManagementPartner](../api/intune-onboarding-compliancemanagementpartner-delete.md)|Nenhum|Exclui um [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md).|
|[Atualizar complianceManagementPartner](../api/intune-onboarding-compliancemanagementpartner-update.md)|[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)|Atualize as propriedades de [um objeto complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|ID da entidade|
|lastHeartbeatDateTime|DateTimeOffset|Carimbo de data/hora da última pulsação depois que o administrador foi integrado ao parceiro de gerenciamento de conformidade|
|partnerState|[deviceManagementPartnerTenantState](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|Estado do parceiro desse locatário. Os possíveis valores são: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.|
|displayName|String|Nome de exibição de parceiro|
|macOsOnboarded|Booliano|Parceiro integrado para dispositivos Mac.|
|androidOnboarded|Boolean|Parceiro integrado para dispositivos Android.|
|iosOnboarded|Booliano|Parceiro integrado para dispositivos ios.|
|macOsEnrollmentAssignments|[coleção complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)|Grupos de usuários que registram dispositivos Mac por meio do parceiro.|
|androidEnrollmentAssignments|[coleção complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)|Grupos de usuários que registram dispositivos Android por meio do parceiro.|
|iosEnrollmentAssignments|[coleção complianceManagementPartnerAssignment](../resources/intune-onboarding-compliancemanagementpartnerassignment.md)|Grupos de usuários que registram dispositivos iOS por meio do parceiro.|

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
  "androidOnboarded": true,
  "iosOnboarded": true,
  "macOsEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "String"
      }
    }
  ],
  "androidEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "String"
      }
    }
  ],
  "iosEnrollmentAssignments": [
    {
      "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "String"
      }
    }
  ]
}
```





