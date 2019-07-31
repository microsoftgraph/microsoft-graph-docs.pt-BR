---
title: tipo de enumeração appListType
description: Valores possíveis da lista de aplicativos de conformidade.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: dca4f368f63296ed2fe751080fcce9c51549b280
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011488"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="83a6b-103">tipo de enumeração appListType</span><span class="sxs-lookup"><span data-stu-id="83a6b-103">appListType enum type</span></span>

> <span data-ttu-id="83a6b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="83a6b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83a6b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="83a6b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83a6b-106">Valores possíveis da lista de aplicativos de conformidade.</span><span class="sxs-lookup"><span data-stu-id="83a6b-106">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="83a6b-107">Membros</span><span class="sxs-lookup"><span data-stu-id="83a6b-107">Members</span></span>
|<span data-ttu-id="83a6b-108">Membro</span><span class="sxs-lookup"><span data-stu-id="83a6b-108">Member</span></span>|<span data-ttu-id="83a6b-109">Valor</span><span class="sxs-lookup"><span data-stu-id="83a6b-109">Value</span></span>|<span data-ttu-id="83a6b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="83a6b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83a6b-111">none</span><span class="sxs-lookup"><span data-stu-id="83a6b-111">none</span></span>|<span data-ttu-id="83a6b-112">,0</span><span class="sxs-lookup"><span data-stu-id="83a6b-112">0</span></span>|<span data-ttu-id="83a6b-113">Valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="83a6b-113">Default value, no intent.</span></span>|
|<span data-ttu-id="83a6b-114">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="83a6b-114">appsInListCompliant</span></span>|<span data-ttu-id="83a6b-115">1</span><span class="sxs-lookup"><span data-stu-id="83a6b-115">1</span></span>|<span data-ttu-id="83a6b-116">A lista representa os aplicativos que serão considerados compatíveis (apenas os aplicativos na lista são compatíveis).</span><span class="sxs-lookup"><span data-stu-id="83a6b-116">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="83a6b-117">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="83a6b-117">appsNotInListCompliant</span></span>|<span data-ttu-id="83a6b-118">duas</span><span class="sxs-lookup"><span data-stu-id="83a6b-118">2</span></span>|<span data-ttu-id="83a6b-119">A lista representa os aplicativos que serão considerados não compatíveis (todos os aplicativos são compatíveis, exceto os aplicativos na lista).</span><span class="sxs-lookup"><span data-stu-id="83a6b-119">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|





