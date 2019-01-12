---
title: tipo de enum appListType
description: Possíveis valores da lista de aplicativos de conformidade.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f1439ab860ab6a1fbf9ff4deb30320bb57fba338
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967235"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="2d208-103">tipo de enum appListType</span><span class="sxs-lookup"><span data-stu-id="2d208-103">appListType enum type</span></span>

> <span data-ttu-id="2d208-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2d208-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2d208-105">Possíveis valores da lista de aplicativos de conformidade.</span><span class="sxs-lookup"><span data-stu-id="2d208-105">Possible values of the compliance app list.</span></span>
## <a name="members"></a><span data-ttu-id="2d208-106">Membros</span><span class="sxs-lookup"><span data-stu-id="2d208-106">Members</span></span>
|<span data-ttu-id="2d208-107">Membro</span><span class="sxs-lookup"><span data-stu-id="2d208-107">Member</span></span>|<span data-ttu-id="2d208-108">Valor</span><span class="sxs-lookup"><span data-stu-id="2d208-108">Value</span></span>|<span data-ttu-id="2d208-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d208-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d208-110">nenhum</span><span class="sxs-lookup"><span data-stu-id="2d208-110">none</span></span>|<span data-ttu-id="2d208-111">0</span><span class="sxs-lookup"><span data-stu-id="2d208-111">0</span></span>|<span data-ttu-id="2d208-112">Valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="2d208-112">Default value, no intent.</span></span>|
|<span data-ttu-id="2d208-113">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="2d208-113">appsInListCompliant</span></span>|<span data-ttu-id="2d208-114">1</span><span class="sxs-lookup"><span data-stu-id="2d208-114">1</span></span>|<span data-ttu-id="2d208-115">A lista representa os aplicativos que serão considerados compatível com (somente aplicativos na lista são compatíveis com).</span><span class="sxs-lookup"><span data-stu-id="2d208-115">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="2d208-116">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="2d208-116">appsNotInListCompliant</span></span>|<span data-ttu-id="2d208-117">2</span><span class="sxs-lookup"><span data-stu-id="2d208-117">2</span></span>|<span data-ttu-id="2d208-118">A lista representa os aplicativos que serão considerados não compatível com (todos os aplicativos são compatíveis, exceto os aplicativos na lista).</span><span class="sxs-lookup"><span data-stu-id="2d208-118">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|



