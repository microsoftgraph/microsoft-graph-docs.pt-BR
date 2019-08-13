---
title: tipo de enumeração appListType
description: Valores possíveis da lista de aplicativos de conformidade.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b9166ef625387b47f07b56efd197dc22f1f440d0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333902"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="edbb6-103">tipo de enumeração appListType</span><span class="sxs-lookup"><span data-stu-id="edbb6-103">appListType enum type</span></span>

> <span data-ttu-id="edbb6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="edbb6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="edbb6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="edbb6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edbb6-106">Valores possíveis da lista de aplicativos de conformidade.</span><span class="sxs-lookup"><span data-stu-id="edbb6-106">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="edbb6-107">Membros</span><span class="sxs-lookup"><span data-stu-id="edbb6-107">Members</span></span>
|<span data-ttu-id="edbb6-108">Membro</span><span class="sxs-lookup"><span data-stu-id="edbb6-108">Member</span></span>|<span data-ttu-id="edbb6-109">Valor</span><span class="sxs-lookup"><span data-stu-id="edbb6-109">Value</span></span>|<span data-ttu-id="edbb6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="edbb6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edbb6-111">none</span><span class="sxs-lookup"><span data-stu-id="edbb6-111">none</span></span>|<span data-ttu-id="edbb6-112">,0</span><span class="sxs-lookup"><span data-stu-id="edbb6-112">0</span></span>|<span data-ttu-id="edbb6-113">Valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="edbb6-113">Default value, no intent.</span></span>|
|<span data-ttu-id="edbb6-114">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="edbb6-114">appsInListCompliant</span></span>|<span data-ttu-id="edbb6-115">1</span><span class="sxs-lookup"><span data-stu-id="edbb6-115">1</span></span>|<span data-ttu-id="edbb6-116">A lista representa os aplicativos que serão considerados compatíveis (apenas os aplicativos na lista são compatíveis).</span><span class="sxs-lookup"><span data-stu-id="edbb6-116">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="edbb6-117">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="edbb6-117">appsNotInListCompliant</span></span>|<span data-ttu-id="edbb6-118">duas</span><span class="sxs-lookup"><span data-stu-id="edbb6-118">2</span></span>|<span data-ttu-id="edbb6-119">A lista representa os aplicativos que serão considerados não compatíveis (todos os aplicativos são compatíveis, exceto os aplicativos na lista).</span><span class="sxs-lookup"><span data-stu-id="edbb6-119">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|



