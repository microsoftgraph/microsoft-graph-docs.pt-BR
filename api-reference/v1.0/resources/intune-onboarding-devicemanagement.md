---
title: Tipo de recurso deviceManagement
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ace2308490e53041fc304fb612db6fbe6948427e
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60455538"
---
# <a name="devicemanagement-resource-type"></a>Tipo de recurso deviceManagement

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceManagement](../api/intune-onboarding-devicemanagement-get.md)|[deviceManagement](../resources/intune-onboarding-devicemanagement.md)|Leia as propriedades e as relações do objeto [deviceManagement](../resources/intune-onboarding-devicemanagement.md).|
|[Atualizar deviceManagement](../api/intune-onboarding-devicemanagement-update.md)|[deviceManagement](../resources/intune-onboarding-devicemanagement.md)|Atualiza as propriedades de um objeto [deviceManagement](../resources/intune-onboarding-devicemanagement.md).|
|[Função verifyWindowsEnrollmentAutoDiscovery](../api/intune-onboarding-devicemanagement-verifywindowsenrollmentautodiscovery.md)|Booliano|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo dessa entidade|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|deviceCategories|Coleção [deviceCategory](../resources/intune-onboarding-devicecategory.md)|A lista de categorias de dispositivo com o locatário.|
|exchangeConnectors|Coleção [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|A lista dos Conectores do Exchange configurados pelo locatário.|
|deviceEnrollmentConfigurations|Coleção [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|A lista de configurações de registro de dispositivos|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|As configurações de acesso condicional do Exchange no local. O acesso condicional no local exigirá que os dispositivos sejam registrados e estejam em conformidade para o acesso ao email|
|mobileThreatDefenseConnectors|Coleção [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)|A lista dos conectores de defesa contra ameaças móveis configurados pelo locatário.|
|deviceManagementPartners|Coleção [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)|A lista de Parceiros de gerenciamento de dispositivos configurados pelo locatário.|
|complianceManagementPartners|[coleção complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)|A lista de Parceiros de Gerenciamento de Conformidade configurados pelo locatário.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "intuneBrand": {
    "@odata.type": "microsoft.graph.intuneBrand",
    "displayName": "String",
    "themeColor": {
      "@odata.type": "microsoft.graph.rgbColor",
      "r": 1024,
      "g": 1024,
      "b": 1024
    },
    "showLogo": true,
    "lightBackgroundLogo": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "String",
      "value": "binary"
    },
    "darkBackgroundLogo": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "String",
      "value": "binary"
    },
    "showNameNextToLogo": true,
    "showDisplayNameNextToLogo": true,
    "contactITName": "String",
    "contactITPhoneNumber": "String",
    "contactITEmailAddress": "String",
    "contactITNotes": "String",
    "onlineSupportSiteUrl": "String",
    "onlineSupportSiteName": "String",
    "privacyUrl": "String"
  }
}
```



