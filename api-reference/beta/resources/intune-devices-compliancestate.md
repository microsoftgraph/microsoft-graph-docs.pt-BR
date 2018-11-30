---
title: tipo de enum complianceState
description: Estado de conformidade.
ms.openlocfilehash: c49c0ecc2511f612e743fb5d86a53d150d3fbf45
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039423"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="21e54-103">tipo de enum complianceState</span><span class="sxs-lookup"><span data-stu-id="21e54-103">complianceState enum type</span></span>

> <span data-ttu-id="21e54-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="21e54-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21e54-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="21e54-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="21e54-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="21e54-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21e54-107">Estado de conformidade.</span><span class="sxs-lookup"><span data-stu-id="21e54-107">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="21e54-108">Membros</span><span class="sxs-lookup"><span data-stu-id="21e54-108">Members</span></span>
|<span data-ttu-id="21e54-109">Membro</span><span class="sxs-lookup"><span data-stu-id="21e54-109">Member</span></span>|<span data-ttu-id="21e54-110">Valor</span><span class="sxs-lookup"><span data-stu-id="21e54-110">Value</span></span>|<span data-ttu-id="21e54-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="21e54-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21e54-112">unknown</span><span class="sxs-lookup"><span data-stu-id="21e54-112">unknown</span></span>|<span data-ttu-id="21e54-113">0</span><span class="sxs-lookup"><span data-stu-id="21e54-113">0</span></span>|<span data-ttu-id="21e54-114">Desconhecido.</span><span class="sxs-lookup"><span data-stu-id="21e54-114">Unknown.</span></span>|
|<span data-ttu-id="21e54-115">compatível com</span><span class="sxs-lookup"><span data-stu-id="21e54-115">compliant</span></span>|<span data-ttu-id="21e54-116">1</span><span class="sxs-lookup"><span data-stu-id="21e54-116">1</span></span>|<span data-ttu-id="21e54-117">Compatível com.</span><span class="sxs-lookup"><span data-stu-id="21e54-117">Compliant.</span></span>|
|<span data-ttu-id="21e54-118">fora de conformidade</span><span class="sxs-lookup"><span data-stu-id="21e54-118">noncompliant</span></span>|<span data-ttu-id="21e54-119">2</span><span class="sxs-lookup"><span data-stu-id="21e54-119">2</span></span>|<span data-ttu-id="21e54-120">Dispositivo não está em conformidade e seja bloqueado para recursos corporativos.</span><span class="sxs-lookup"><span data-stu-id="21e54-120">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="21e54-121">conflito</span><span class="sxs-lookup"><span data-stu-id="21e54-121">conflict</span></span>|<span data-ttu-id="21e54-122">3</span><span class="sxs-lookup"><span data-stu-id="21e54-122">3</span></span>|<span data-ttu-id="21e54-123">Conflito com outras regras.</span><span class="sxs-lookup"><span data-stu-id="21e54-123">Conflict with other rules.</span></span>|
|<span data-ttu-id="21e54-124">erro</span><span class="sxs-lookup"><span data-stu-id="21e54-124">error</span></span>|<span data-ttu-id="21e54-125">4</span><span class="sxs-lookup"><span data-stu-id="21e54-125">4</span></span>|<span data-ttu-id="21e54-126">Erro</span><span class="sxs-lookup"><span data-stu-id="21e54-126">Error.</span></span>|
|<span data-ttu-id="21e54-127">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="21e54-127">inGracePeriod</span></span>|<span data-ttu-id="21e54-128">254</span><span class="sxs-lookup"><span data-stu-id="21e54-128">254</span></span>|<span data-ttu-id="21e54-129">Dispositivo não está em conformidade, mas ainda tem acesso aos recursos corporativos</span><span class="sxs-lookup"><span data-stu-id="21e54-129">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="21e54-130">configManager</span><span class="sxs-lookup"><span data-stu-id="21e54-130">configManager</span></span>|<span data-ttu-id="21e54-131">255</span><span class="sxs-lookup"><span data-stu-id="21e54-131">255</span></span>|<span data-ttu-id="21e54-132">Gerenciado pelo Gerenciador de configuração</span><span class="sxs-lookup"><span data-stu-id="21e54-132">Managed by Config Manager</span></span>|





