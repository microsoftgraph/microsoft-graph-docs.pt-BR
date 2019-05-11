---
title: tipo de recurso adminConsent
description: Informações de consentimento do administrador.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aaac2bb11d90f1e6fec52fae0c17f374c33868ce
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943365"
---
# <a name="adminconsent-resource-type"></a>tipo de recurso adminConsent

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Informações de consentimento do administrador.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|shareAPNSData|[adminConsentState](../resources/intune-devices-adminconsentstate.md)|O estado de consentimento do administrador do compartilhamento de dados de usuário e de dispositivo para a Apple. Os valores possíveis são: `notConfigured`, `granted`, `notGranted`.|

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
  "shareAPNSData": "String"
}
```




