---
title: Tipo de recurso aadUserNotificationRecipient
description: Representa um Azure Active Directory (Azure AD) destinatário de uma notificação enviada em um feed Microsoft Teams atividade.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ec8e05a09af27ca6092da24e13a604fdd7e013f4
ms.sourcegitcommit: a2d81138de2a0404e611fbb535679199477ef3d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2021
ms.locfileid: "52813192"
---
# <a name="aadusernotificationrecipient-resource-type"></a>Tipo de recurso aadUserNotificationRecipient

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um Azure Active Directory (Azure AD) destinatário de uma notificação enviada em um feed Microsoft Teams atividade.

Herda de [teamworkNotificationRecipient](teamworknotificationrecipient.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|userId|Cadeia de caracteres|Identificador de usuário do Azure AD. Use o [método List users](../api/user-list.md) para obter essa ID.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.aadUserNotificationRecipient"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.aadUserNotificationRecipient",
  "userId": "String"
}
```

