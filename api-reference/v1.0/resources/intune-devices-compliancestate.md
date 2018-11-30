---
title: tipo de enum complianceState
description: Estado de conformidade.
ms.openlocfilehash: 041a2267b952d37e0aeef29e1325e5cb7b561ed7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006883"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="4849a-103">tipo de enum complianceState</span><span class="sxs-lookup"><span data-stu-id="4849a-103">complianceState enum type</span></span>

> <span data-ttu-id="4849a-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4849a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4849a-105">Estado de conformidade.</span><span class="sxs-lookup"><span data-stu-id="4849a-105">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="4849a-106">Membros</span><span class="sxs-lookup"><span data-stu-id="4849a-106">Members</span></span>
|<span data-ttu-id="4849a-107">Membro</span><span class="sxs-lookup"><span data-stu-id="4849a-107">Member</span></span>|<span data-ttu-id="4849a-108">Valor</span><span class="sxs-lookup"><span data-stu-id="4849a-108">Value</span></span>|<span data-ttu-id="4849a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="4849a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4849a-110">unknown</span><span class="sxs-lookup"><span data-stu-id="4849a-110">unknown</span></span>|<span data-ttu-id="4849a-111">0</span><span class="sxs-lookup"><span data-stu-id="4849a-111">0</span></span>|<span data-ttu-id="4849a-112">Desconhecido.</span><span class="sxs-lookup"><span data-stu-id="4849a-112">Unknown.</span></span>|
|<span data-ttu-id="4849a-113">compatível com</span><span class="sxs-lookup"><span data-stu-id="4849a-113">compliant</span></span>|<span data-ttu-id="4849a-114">1</span><span class="sxs-lookup"><span data-stu-id="4849a-114">1</span></span>|<span data-ttu-id="4849a-115">Compatível com.</span><span class="sxs-lookup"><span data-stu-id="4849a-115">Compliant.</span></span>|
|<span data-ttu-id="4849a-116">fora de conformidade</span><span class="sxs-lookup"><span data-stu-id="4849a-116">noncompliant</span></span>|<span data-ttu-id="4849a-117">2</span><span class="sxs-lookup"><span data-stu-id="4849a-117">2</span></span>|<span data-ttu-id="4849a-118">Dispositivo não está em conformidade e seja bloqueado para recursos corporativos.</span><span class="sxs-lookup"><span data-stu-id="4849a-118">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="4849a-119">conflito</span><span class="sxs-lookup"><span data-stu-id="4849a-119">conflict</span></span>|<span data-ttu-id="4849a-120">3</span><span class="sxs-lookup"><span data-stu-id="4849a-120">3</span></span>|<span data-ttu-id="4849a-121">Conflito com outras regras.</span><span class="sxs-lookup"><span data-stu-id="4849a-121">Conflict with other rules.</span></span>|
|<span data-ttu-id="4849a-122">erro</span><span class="sxs-lookup"><span data-stu-id="4849a-122">error</span></span>|<span data-ttu-id="4849a-123">4</span><span class="sxs-lookup"><span data-stu-id="4849a-123">4</span></span>|<span data-ttu-id="4849a-124">Erro</span><span class="sxs-lookup"><span data-stu-id="4849a-124">Error.</span></span>|
|<span data-ttu-id="4849a-125">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="4849a-125">inGracePeriod</span></span>|<span data-ttu-id="4849a-126">254</span><span class="sxs-lookup"><span data-stu-id="4849a-126">254</span></span>|<span data-ttu-id="4849a-127">Dispositivo não está em conformidade, mas ainda tem acesso aos recursos corporativos</span><span class="sxs-lookup"><span data-stu-id="4849a-127">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="4849a-128">configManager</span><span class="sxs-lookup"><span data-stu-id="4849a-128">configManager</span></span>|<span data-ttu-id="4849a-129">255</span><span class="sxs-lookup"><span data-stu-id="4849a-129">255</span></span>|<span data-ttu-id="4849a-130">Gerenciado pelo Gerenciador de configuração</span><span class="sxs-lookup"><span data-stu-id="4849a-130">Managed by Config Manager</span></span>|



