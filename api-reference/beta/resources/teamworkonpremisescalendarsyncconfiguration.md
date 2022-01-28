---
title: tipo de recurso teamworkOnPremisesCalendarSyncConfiguration
description: Representa os detalhes sobre a conta usada para sincronizar calendários Microsoft Teams cliente de um dispositivo habilitado Microsoft Teams usuário.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7b5b8d95cc2743b15c6903852a0d81c41949148a
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262271"
---
# <a name="teamworkonpremisescalendarsyncconfiguration-resource-type"></a>tipo de recurso teamworkOnPremisesCalendarSyncConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes sobre a conta usada para sincronizar calendários Microsoft Teams cliente de um [Microsoft Teams habilitado.](../resources/teamworkdevice.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|domínio|Cadeia de caracteres|O FQDN (nome de domínio totalmente qualificado) do Skype for Business Server. Use o domínio Exchange se o domínio SIP Skype for Business for diferente do domínio Exchange do usuário.|
|domainUserName|Cadeia de caracteres|O domínio e o nome de usuário do dispositivo de console, por exemplo, `Seattle\RanierConf`.|
|smtpAddress|String|O endereço SMTP (Simple Mail Transfer Protocol) da conta de usuário. Isso só será necessário se um nome de entidade de usuário diferente (UPN) for usado para entrar Exchange além de Microsoft Teams e Skype for Business. Esse é um cenário comum em um ambiente híbrido em que um servidor Exchange local é usado.|


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkOnPremisesCalendarSyncConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkOnPremisesCalendarSyncConfiguration",
  "domain": "String",
  "domainUserName": "String",
  "smtpAddress": "String"
}
```

