---
title: Tipo de recurso aadUserNotificationRecipient
description: Representa um Azure Active Directory (Azure AD) destinatário de uma notificação enviada em um feed Microsoft Teams atividade.
author: eddie-lee-msft
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4588b0d17dc099ee65cedeba52bd5cbd1edf7bae
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59021782"
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

