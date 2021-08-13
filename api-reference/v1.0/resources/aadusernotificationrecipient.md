---
title: Tipo de recurso aadUserNotificationRecipient
description: Representa um Azure Active Directory (Azure AD) destinatário de uma notificação enviada em um feed Microsoft Teams atividade.
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: bb5d95c36fb362af6d4f66c1e18a4dcb768c1b204a4e2f70f24f5afe80545483
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54230848"
---
# <a name="aadusernotificationrecipient-resource-type"></a>Tipo de recurso aadUserNotificationRecipient

Namespace: microsoft.graph

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

