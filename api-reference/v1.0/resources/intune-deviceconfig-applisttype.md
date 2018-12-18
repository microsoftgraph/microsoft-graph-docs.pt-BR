---
title: tipo de enum appListType
description: Possíveis valores da lista de aplicativos de conformidade.
author: tfitzmac
ms.openlocfilehash: ab5d8f45343b017693906b13be25c88d5b06e8f7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354716"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="52759-103">tipo de enum appListType</span><span class="sxs-lookup"><span data-stu-id="52759-103">appListType enum type</span></span>

> <span data-ttu-id="52759-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="52759-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="52759-105">Possíveis valores da lista de aplicativos de conformidade.</span><span class="sxs-lookup"><span data-stu-id="52759-105">Possible values of the compliance app list.</span></span>
## <a name="members"></a><span data-ttu-id="52759-106">Membros</span><span class="sxs-lookup"><span data-stu-id="52759-106">Members</span></span>
|<span data-ttu-id="52759-107">Membro</span><span class="sxs-lookup"><span data-stu-id="52759-107">Member</span></span>|<span data-ttu-id="52759-108">Valor</span><span class="sxs-lookup"><span data-stu-id="52759-108">Value</span></span>|<span data-ttu-id="52759-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="52759-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52759-110">none</span><span class="sxs-lookup"><span data-stu-id="52759-110">none</span></span>|<span data-ttu-id="52759-111">0</span><span class="sxs-lookup"><span data-stu-id="52759-111">0</span></span>|<span data-ttu-id="52759-112">Valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="52759-112">Default value, no intent.</span></span>|
|<span data-ttu-id="52759-113">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="52759-113">appsInListCompliant</span></span>|<span data-ttu-id="52759-114">1</span><span class="sxs-lookup"><span data-stu-id="52759-114">1</span></span>|<span data-ttu-id="52759-115">A lista representa os aplicativos que serão considerados compatível com (somente aplicativos na lista são compatíveis com).</span><span class="sxs-lookup"><span data-stu-id="52759-115">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="52759-116">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="52759-116">appsNotInListCompliant</span></span>|<span data-ttu-id="52759-117">2</span><span class="sxs-lookup"><span data-stu-id="52759-117">2</span></span>|<span data-ttu-id="52759-118">A lista representa os aplicativos que serão considerados não compatível com (todos os aplicativos são compatíveis, exceto os aplicativos na lista).</span><span class="sxs-lookup"><span data-stu-id="52759-118">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|



