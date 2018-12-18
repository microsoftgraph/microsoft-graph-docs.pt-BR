---
title: tipo de enum vpnTrafficRuleAppType
description: Indica o tipo de aplicativo que uma regra de tráfego VPN está associada.
author: tfitzmac
ms.openlocfilehash: 3ab20bf62029e57c93c80d5f49d964abb58a883d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347352"
---
# <a name="vpntrafficruleapptype-enum-type"></a><span data-ttu-id="0b314-103">tipo de enum vpnTrafficRuleAppType</span><span class="sxs-lookup"><span data-stu-id="0b314-103">vpnTrafficRuleAppType enum type</span></span>

> <span data-ttu-id="0b314-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0b314-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0b314-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0b314-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0b314-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0b314-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0b314-107">Indica o tipo de aplicativo que uma regra de tráfego VPN está associada.</span><span class="sxs-lookup"><span data-stu-id="0b314-107">Indicates the type of app that a VPN traffic rule is associated with.</span></span>
## <a name="members"></a><span data-ttu-id="0b314-108">Membros</span><span class="sxs-lookup"><span data-stu-id="0b314-108">Members</span></span>
|<span data-ttu-id="0b314-109">Membro</span><span class="sxs-lookup"><span data-stu-id="0b314-109">Member</span></span>|<span data-ttu-id="0b314-110">Valor</span><span class="sxs-lookup"><span data-stu-id="0b314-110">Value</span></span>|<span data-ttu-id="0b314-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b314-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b314-112">none</span><span class="sxs-lookup"><span data-stu-id="0b314-112">none</span></span>|<span data-ttu-id="0b314-113">0</span><span class="sxs-lookup"><span data-stu-id="0b314-113">0</span></span>|<span data-ttu-id="0b314-114">A regra de tráfego não está associada um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0b314-114">The traffic rule is not associated with an app.</span></span>|
|<span data-ttu-id="0b314-115">área de trabalho</span><span class="sxs-lookup"><span data-stu-id="0b314-115">desktop</span></span>|<span data-ttu-id="0b314-116">1</span><span class="sxs-lookup"><span data-stu-id="0b314-116">1</span></span>|<span data-ttu-id="0b314-117">A regra de tráfego é associada um aplicativo de área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="0b314-117">The traffic rule is associated with a desktop app.</span></span>|
|<span data-ttu-id="0b314-118">universal</span><span class="sxs-lookup"><span data-stu-id="0b314-118">universal</span></span>|<span data-ttu-id="0b314-119">2</span><span class="sxs-lookup"><span data-stu-id="0b314-119">2</span></span>|<span data-ttu-id="0b314-120">A regra de tráfego é associada um aplicativo Universal.</span><span class="sxs-lookup"><span data-stu-id="0b314-120">The traffic rule is associated with a Universal app.</span></span>|





