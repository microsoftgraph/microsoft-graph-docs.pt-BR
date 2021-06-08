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
# <a name="aadusernotificationrecipient-resource-type"></a><span data-ttu-id="10d60-103">Tipo de recurso aadUserNotificationRecipient</span><span class="sxs-lookup"><span data-stu-id="10d60-103">aadUserNotificationRecipient resource type</span></span>

<span data-ttu-id="10d60-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10d60-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10d60-105">Representa um Azure Active Directory (Azure AD) destinatário de uma notificação enviada em um feed Microsoft Teams atividade.</span><span class="sxs-lookup"><span data-stu-id="10d60-105">Represents an Azure Active Directory (Azure AD) user recipient of a notification sent in a Microsoft Teams activity feed.</span></span>

<span data-ttu-id="10d60-106">Herda de [teamworkNotificationRecipient](teamworknotificationrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="10d60-106">Inherits from [teamworkNotificationRecipient](teamworknotificationrecipient.md).</span></span>

## <a name="properties"></a><span data-ttu-id="10d60-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="10d60-107">Properties</span></span>
|<span data-ttu-id="10d60-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10d60-108">Property</span></span>|<span data-ttu-id="10d60-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="10d60-109">Type</span></span>|<span data-ttu-id="10d60-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="10d60-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10d60-111">userId</span><span class="sxs-lookup"><span data-stu-id="10d60-111">userId</span></span>|<span data-ttu-id="10d60-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10d60-112">String</span></span>|<span data-ttu-id="10d60-113">Identificador de usuário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="10d60-113">Azure AD user identifier.</span></span> <span data-ttu-id="10d60-114">Use o [método List users](../api/user-list.md) para obter essa ID.</span><span class="sxs-lookup"><span data-stu-id="10d60-114">Use the [List users](../api/user-list.md) method to get this ID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="10d60-115">Relações</span><span class="sxs-lookup"><span data-stu-id="10d60-115">Relationships</span></span>
<span data-ttu-id="10d60-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="10d60-116">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="10d60-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="10d60-117">JSON representation</span></span>
<span data-ttu-id="10d60-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="10d60-118">The following is a JSON representation of the resource.</span></span>
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

