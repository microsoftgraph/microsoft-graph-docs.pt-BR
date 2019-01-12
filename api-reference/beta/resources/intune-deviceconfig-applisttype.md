---
title: tipo de enum appListType
description: Possíveis valores da lista de aplicativos de conformidade.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: eb2b4afa6639d70b81a59bda1250ea9ed231ccdb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939641"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="22d04-103">tipo de enum appListType</span><span class="sxs-lookup"><span data-stu-id="22d04-103">appListType enum type</span></span>

> <span data-ttu-id="22d04-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="22d04-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22d04-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="22d04-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="22d04-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="22d04-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="22d04-107">Possíveis valores da lista de aplicativos de conformidade.</span><span class="sxs-lookup"><span data-stu-id="22d04-107">Possible values of the compliance app list.</span></span>
## <a name="members"></a><span data-ttu-id="22d04-108">Membros</span><span class="sxs-lookup"><span data-stu-id="22d04-108">Members</span></span>
|<span data-ttu-id="22d04-109">Membro</span><span class="sxs-lookup"><span data-stu-id="22d04-109">Member</span></span>|<span data-ttu-id="22d04-110">Valor</span><span class="sxs-lookup"><span data-stu-id="22d04-110">Value</span></span>|<span data-ttu-id="22d04-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="22d04-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22d04-112">nenhum</span><span class="sxs-lookup"><span data-stu-id="22d04-112">none</span></span>|<span data-ttu-id="22d04-113">0</span><span class="sxs-lookup"><span data-stu-id="22d04-113">0</span></span>|<span data-ttu-id="22d04-114">Valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="22d04-114">Default value, no intent.</span></span>|
|<span data-ttu-id="22d04-115">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="22d04-115">appsInListCompliant</span></span>|<span data-ttu-id="22d04-116">1</span><span class="sxs-lookup"><span data-stu-id="22d04-116">1</span></span>|<span data-ttu-id="22d04-117">A lista representa os aplicativos que serão considerados compatível com (somente aplicativos na lista são compatíveis com).</span><span class="sxs-lookup"><span data-stu-id="22d04-117">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="22d04-118">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="22d04-118">appsNotInListCompliant</span></span>|<span data-ttu-id="22d04-119">2</span><span class="sxs-lookup"><span data-stu-id="22d04-119">2</span></span>|<span data-ttu-id="22d04-120">A lista representa os aplicativos que serão considerados não compatível com (todos os aplicativos são compatíveis, exceto os aplicativos na lista).</span><span class="sxs-lookup"><span data-stu-id="22d04-120">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|





