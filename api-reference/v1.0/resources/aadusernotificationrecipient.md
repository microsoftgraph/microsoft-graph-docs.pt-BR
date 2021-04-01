---
title: Tipo de recurso aadUserNotificationRecipient
description: Representa um destinatário de usuário do Azure Active Directory (Azure AD) de uma notificação enviada em um feed de atividades do Microsoft Teams.
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: dadb08dad99f6c4fd6857e8e60f457ea51811de1
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51474115"
---
# <a name="aadusernotificationrecipient-resource-type"></a>Tipo de recurso aadUserNotificationRecipient

Namespace: microsoft.graph

Representa um destinatário de usuário do Azure Active Directory (Azure AD) de uma notificação enviada em um feed de atividades do Microsoft Teams.

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

