---
title: tipo de recurso aadUserNotificationRecipient
description: Representa um destinatário do usuário do Azure Active Directory (Azure AD) de uma notificação enviada em um feed de atividades do Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 118951336a031548a557f94df8b2b2068e415408
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377486"
---
# <a name="aadusernotificationrecipient-resource-type"></a>tipo de recurso aadUserNotificationRecipient

Namespace: microsoft.graph

Representa um destinatário do usuário do Azure Active Directory (Azure AD) de uma notificação enviada em um feed de atividades do Microsoft Teams.

Herda de [teamworkNotificationRecipient](teamworknotificationrecipient.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|userId|Cadeia de caracteres|Identificador de usuário do Azure AD. Use o método [list Users](../api/user-list.md) para obter essa ID.|

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

