---
title: tipo de enum appListType
description: Possíveis valores da lista de aplicativos de conformidade.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 17452d09976d84f19ed56bbaeb4e558a727b1c7c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841017"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="06014-103">tipo de enum appListType</span><span class="sxs-lookup"><span data-stu-id="06014-103">appListType enum type</span></span>

> <span data-ttu-id="06014-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="06014-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06014-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="06014-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06014-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="06014-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06014-107">Possíveis valores da lista de aplicativos de conformidade.</span><span class="sxs-lookup"><span data-stu-id="06014-107">Possible values of the compliance app list.</span></span>
## <a name="members"></a><span data-ttu-id="06014-108">Membros</span><span class="sxs-lookup"><span data-stu-id="06014-108">Members</span></span>
|<span data-ttu-id="06014-109">Membro</span><span class="sxs-lookup"><span data-stu-id="06014-109">Member</span></span>|<span data-ttu-id="06014-110">Valor</span><span class="sxs-lookup"><span data-stu-id="06014-110">Value</span></span>|<span data-ttu-id="06014-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="06014-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06014-112">nenhum</span><span class="sxs-lookup"><span data-stu-id="06014-112">none</span></span>|<span data-ttu-id="06014-113">0</span><span class="sxs-lookup"><span data-stu-id="06014-113">0</span></span>|<span data-ttu-id="06014-114">Valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="06014-114">Default value, no intent.</span></span>|
|<span data-ttu-id="06014-115">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="06014-115">appsInListCompliant</span></span>|<span data-ttu-id="06014-116">1</span><span class="sxs-lookup"><span data-stu-id="06014-116">1</span></span>|<span data-ttu-id="06014-117">A lista representa os aplicativos que serão considerados compatível com (somente aplicativos na lista são compatíveis com).</span><span class="sxs-lookup"><span data-stu-id="06014-117">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="06014-118">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="06014-118">appsNotInListCompliant</span></span>|<span data-ttu-id="06014-119">2</span><span class="sxs-lookup"><span data-stu-id="06014-119">2</span></span>|<span data-ttu-id="06014-120">A lista representa os aplicativos que serão considerados não compatível com (todos os aplicativos são compatíveis, exceto os aplicativos na lista).</span><span class="sxs-lookup"><span data-stu-id="06014-120">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|





