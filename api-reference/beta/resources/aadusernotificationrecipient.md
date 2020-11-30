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
# <a name="aadusernotificationrecipient-resource-type"></a><span data-ttu-id="021a3-103">tipo de recurso aadUserNotificationRecipient</span><span class="sxs-lookup"><span data-stu-id="021a3-103">aadUserNotificationRecipient resource type</span></span>

<span data-ttu-id="021a3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="021a3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="021a3-105">Representa um destinatário do usuário do Azure Active Directory (Azure AD) de uma notificação enviada em um feed de atividades do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="021a3-105">Represents an Azure Active Directory (Azure AD) user recipient of a notification sent in a Microsoft Teams activity feed.</span></span>

<span data-ttu-id="021a3-106">Herda de [teamworkNotificationRecipient](teamworknotificationrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="021a3-106">Inherits from [teamworkNotificationRecipient](teamworknotificationrecipient.md).</span></span>

## <a name="properties"></a><span data-ttu-id="021a3-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="021a3-107">Properties</span></span>
|<span data-ttu-id="021a3-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="021a3-108">Property</span></span>|<span data-ttu-id="021a3-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="021a3-109">Type</span></span>|<span data-ttu-id="021a3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="021a3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="021a3-111">userId</span><span class="sxs-lookup"><span data-stu-id="021a3-111">userId</span></span>|<span data-ttu-id="021a3-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="021a3-112">String</span></span>|<span data-ttu-id="021a3-113">Identificador de usuário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="021a3-113">Azure AD user identifier.</span></span> <span data-ttu-id="021a3-114">Use o método [list Users](../api/user-list.md) para obter essa ID.</span><span class="sxs-lookup"><span data-stu-id="021a3-114">Use the [List users](../api/user-list.md) method to get this ID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="021a3-115">Relações</span><span class="sxs-lookup"><span data-stu-id="021a3-115">Relationships</span></span>
<span data-ttu-id="021a3-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="021a3-116">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="021a3-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="021a3-117">JSON representation</span></span>
<span data-ttu-id="021a3-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="021a3-118">The following is a JSON representation of the resource.</span></span>
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

