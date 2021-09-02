---
title: Tipo de recurso adminConsent
description: Informações de consentimento do administrador.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dcf849e8c44e68bb4b76417748dbe795e0dd5852
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58816512"
---
# <a name="adminconsent-resource-type"></a>Tipo de recurso adminConsent

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Informações de consentimento do administrador.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|shareAPNSData|[adminConsentState](../resources/intune-devices-adminconsentstate.md)|O estado de consentimento do administrador de compartilhamento de dados de usuário e dispositivo para a Apple. Os valores possíveis são: `notConfigured`, `granted`, `notGranted`.|
|shareUserExperienceAnalyticsData|[adminConsentState](../resources/intune-devices-adminconsentstate.md)|Obtém ou define o consentimento do administrador para compartilhar dados de análise de experiência do usuário. Os valores possíveis são: `notConfigured`, `granted`, `notGranted`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.adminConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminConsent",
  "shareAPNSData": "String",
  "shareUserExperienceAnalyticsData": "String"
}
```



