---
title: Tipo de recurso deviceManagementPartner
description: Entidade que representa uma conexão ao parceiro de gerenciamento de dispositivos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0df0f36c5a8747e3be3b3ab800c267680d6a532f
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156774"
---
# <a name="devicemanagementpartner-resource-type"></a>Tipo de recurso deviceManagementPartner

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa uma conexão ao parceiro de gerenciamento de dispositivos.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementPartners](../api/intune-onboarding-devicemanagementpartner-list.md)|Conjunto [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)|Listar propriedades e relações de objetos de [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).|
|[Obter deviceManagementPartner](../api/intune-onboarding-devicemanagementpartner-get.md)|[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)|Ler propriedades e relações de objetos de [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).|
|[Criar deviceManagementPartner](../api/intune-onboarding-devicemanagementpartner-create.md)|[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)|Crie um novo objeto de [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).|
|[Excluir deviceManagementPartner](../api/intune-onboarding-devicemanagementpartner-delete.md)|Nenhum|Excluir [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).|
|[Atualizar deviceManagementPartner](../api/intune-onboarding-devicemanagementpartner-update.md)|[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)|Atualizar as propriedades de um objeto de [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|ID da entidade|
|lastHeartbeatDateTime|DateTimeOffset|Carimbo de data/hora da última pulsação após a opção de administrador habilitado conectar-se ao parceiro de gerenciamento de dispositivo|
|partnerState|[deviceManagementPartnerTenantState](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|Estado do parceiro deste locatário. Os possíveis valores são: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.|
|partnerAppType|[deviceManagementPartnerAppType](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|Tipo de aplicativo parceiro. Os valores possíveis são: `unknown`, `singleTenantApp`, `multiTenantApp`.|
|singleTenantAppId|Cadeia de caracteres|Id do aplicativo do único locatário do parceiro|
|displayName|String|Nome de exibição de parceiro|
|isConfigured|Booliano|Se o parceiro de gerenciamento de dispositivo está configurado ou não|
|whenPartnerDevicesWillBeRemoved|DateTimeOffset|DateTime em UTC quando PartnerDevices será removido. Isso se tornará obselete em breve.|
|whenPartnerDevicesWillBeMarkedAsNonCompliant|DateTimeOffset|DateTime em UTC quando PartnerDevices será marcado como Não Compatível. Isso se tornará obselete em breve.|
|whenPartnerDevicesWillBeRemovedDateTime|DateTimeOffset|DateTime no UTC quando PartnerDevices for removido|
|whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime|DateTimeOffset|DateTime no UTC quando PartnerDevices for marcado como não compatível|
|groupsRequiringPartnerEnrollment|[Coleção deviceManagementPartnerAssignment](../resources/intune-onboarding-devicemanagementpartnerassignment.md)|Grupos de usuários que especificam se o registro é por meio do parceiro.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementPartner"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "String (identifier)",
  "lastHeartbeatDateTime": "String (timestamp)",
  "partnerState": "String",
  "partnerAppType": "String",
  "singleTenantAppId": "String",
  "displayName": "String",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemoved": "String (timestamp)",
  "whenPartnerDevicesWillBeMarkedAsNonCompliant": "String (timestamp)",
  "whenPartnerDevicesWillBeRemovedDateTime": "String (timestamp)",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "String (timestamp)",
  "groupsRequiringPartnerEnrollment": [
    {
      "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment",
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




