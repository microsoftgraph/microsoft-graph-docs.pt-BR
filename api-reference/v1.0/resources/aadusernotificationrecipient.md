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
# <a name="aadusernotificationrecipient-resource-type"></a><span data-ttu-id="d2fdb-103">Tipo de recurso aadUserNotificationRecipient</span><span class="sxs-lookup"><span data-stu-id="d2fdb-103">aadUserNotificationRecipient resource type</span></span>

<span data-ttu-id="d2fdb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2fdb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d2fdb-105">Representa um destinatário de usuário do Azure Active Directory (Azure AD) de uma notificação enviada em um feed de atividades do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="d2fdb-105">Represents an Azure Active Directory (Azure AD) user recipient of a notification sent in a Microsoft Teams activity feed.</span></span>

<span data-ttu-id="d2fdb-106">Herda de [teamworkNotificationRecipient](teamworknotificationrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="d2fdb-106">Inherits from [teamworkNotificationRecipient](teamworknotificationrecipient.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d2fdb-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d2fdb-107">Properties</span></span>
|<span data-ttu-id="d2fdb-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2fdb-108">Property</span></span>|<span data-ttu-id="d2fdb-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2fdb-109">Type</span></span>|<span data-ttu-id="d2fdb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2fdb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2fdb-111">userId</span><span class="sxs-lookup"><span data-stu-id="d2fdb-111">userId</span></span>|<span data-ttu-id="d2fdb-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d2fdb-112">String</span></span>|<span data-ttu-id="d2fdb-113">Identificador de usuário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d2fdb-113">Azure AD user identifier.</span></span> <span data-ttu-id="d2fdb-114">Use o [método List users](../api/user-list.md) para obter essa ID.</span><span class="sxs-lookup"><span data-stu-id="d2fdb-114">Use the [List users](../api/user-list.md) method to get this ID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2fdb-115">Relações</span><span class="sxs-lookup"><span data-stu-id="d2fdb-115">Relationships</span></span>
<span data-ttu-id="d2fdb-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d2fdb-116">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2fdb-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d2fdb-117">JSON representation</span></span>
<span data-ttu-id="d2fdb-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d2fdb-118">The following is a JSON representation of the resource.</span></span>
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

