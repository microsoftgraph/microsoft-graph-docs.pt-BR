---
title: tipo de enum appListType
description: Possíveis valores da lista de aplicativos de conformidade.
author: tfitzmac
ms.openlocfilehash: 3f0fa162131fc1f59beba1f057fa888e0f2260c5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331189"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="b4113-103">tipo de enum appListType</span><span class="sxs-lookup"><span data-stu-id="b4113-103">appListType enum type</span></span>

> <span data-ttu-id="b4113-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b4113-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b4113-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b4113-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b4113-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b4113-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4113-107">Possíveis valores da lista de aplicativos de conformidade.</span><span class="sxs-lookup"><span data-stu-id="b4113-107">Possible values of the compliance app list.</span></span>
## <a name="members"></a><span data-ttu-id="b4113-108">Membros</span><span class="sxs-lookup"><span data-stu-id="b4113-108">Members</span></span>
|<span data-ttu-id="b4113-109">Membro</span><span class="sxs-lookup"><span data-stu-id="b4113-109">Member</span></span>|<span data-ttu-id="b4113-110">Valor</span><span class="sxs-lookup"><span data-stu-id="b4113-110">Value</span></span>|<span data-ttu-id="b4113-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4113-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4113-112">none</span><span class="sxs-lookup"><span data-stu-id="b4113-112">none</span></span>|<span data-ttu-id="b4113-113">0</span><span class="sxs-lookup"><span data-stu-id="b4113-113">0</span></span>|<span data-ttu-id="b4113-114">Valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="b4113-114">Default value, no intent.</span></span>|
|<span data-ttu-id="b4113-115">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="b4113-115">appsInListCompliant</span></span>|<span data-ttu-id="b4113-116">1</span><span class="sxs-lookup"><span data-stu-id="b4113-116">1</span></span>|<span data-ttu-id="b4113-117">A lista representa os aplicativos que serão considerados compatível com (somente aplicativos na lista são compatíveis com).</span><span class="sxs-lookup"><span data-stu-id="b4113-117">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="b4113-118">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="b4113-118">appsNotInListCompliant</span></span>|<span data-ttu-id="b4113-119">2</span><span class="sxs-lookup"><span data-stu-id="b4113-119">2</span></span>|<span data-ttu-id="b4113-120">A lista representa os aplicativos que serão considerados não compatível com (todos os aplicativos são compatíveis, exceto os aplicativos na lista).</span><span class="sxs-lookup"><span data-stu-id="b4113-120">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|





