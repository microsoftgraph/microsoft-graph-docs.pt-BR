---
title: tipo de enum complianceState
description: Estado de conformidade.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b3d496d6890d0da4d817ad9ba1f03e4b0825204d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861674"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="2e859-103">tipo de enum complianceState</span><span class="sxs-lookup"><span data-stu-id="2e859-103">complianceState enum type</span></span>

> <span data-ttu-id="2e859-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2e859-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2e859-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2e859-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2e859-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2e859-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2e859-107">Estado de conformidade.</span><span class="sxs-lookup"><span data-stu-id="2e859-107">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="2e859-108">Membros</span><span class="sxs-lookup"><span data-stu-id="2e859-108">Members</span></span>
|<span data-ttu-id="2e859-109">Membro</span><span class="sxs-lookup"><span data-stu-id="2e859-109">Member</span></span>|<span data-ttu-id="2e859-110">Valor</span><span class="sxs-lookup"><span data-stu-id="2e859-110">Value</span></span>|<span data-ttu-id="2e859-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e859-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e859-112">unknown</span><span class="sxs-lookup"><span data-stu-id="2e859-112">unknown</span></span>|<span data-ttu-id="2e859-113">0</span><span class="sxs-lookup"><span data-stu-id="2e859-113">0</span></span>|<span data-ttu-id="2e859-114">Desconhecido.</span><span class="sxs-lookup"><span data-stu-id="2e859-114">Unknown.</span></span>|
|<span data-ttu-id="2e859-115">compatível com</span><span class="sxs-lookup"><span data-stu-id="2e859-115">compliant</span></span>|<span data-ttu-id="2e859-116">1</span><span class="sxs-lookup"><span data-stu-id="2e859-116">1</span></span>|<span data-ttu-id="2e859-117">Compatível com.</span><span class="sxs-lookup"><span data-stu-id="2e859-117">Compliant.</span></span>|
|<span data-ttu-id="2e859-118">fora de conformidade</span><span class="sxs-lookup"><span data-stu-id="2e859-118">noncompliant</span></span>|<span data-ttu-id="2e859-119">2</span><span class="sxs-lookup"><span data-stu-id="2e859-119">2</span></span>|<span data-ttu-id="2e859-120">Dispositivo não está em conformidade e seja bloqueado para recursos corporativos.</span><span class="sxs-lookup"><span data-stu-id="2e859-120">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="2e859-121">conflito</span><span class="sxs-lookup"><span data-stu-id="2e859-121">conflict</span></span>|<span data-ttu-id="2e859-122">3</span><span class="sxs-lookup"><span data-stu-id="2e859-122">3</span></span>|<span data-ttu-id="2e859-123">Conflito com outras regras.</span><span class="sxs-lookup"><span data-stu-id="2e859-123">Conflict with other rules.</span></span>|
|<span data-ttu-id="2e859-124">erro</span><span class="sxs-lookup"><span data-stu-id="2e859-124">error</span></span>|<span data-ttu-id="2e859-125">4</span><span class="sxs-lookup"><span data-stu-id="2e859-125">4</span></span>|<span data-ttu-id="2e859-126">Erro</span><span class="sxs-lookup"><span data-stu-id="2e859-126">Error.</span></span>|
|<span data-ttu-id="2e859-127">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="2e859-127">inGracePeriod</span></span>|<span data-ttu-id="2e859-128">254</span><span class="sxs-lookup"><span data-stu-id="2e859-128">254</span></span>|<span data-ttu-id="2e859-129">Dispositivo não está em conformidade, mas ainda tem acesso aos recursos corporativos</span><span class="sxs-lookup"><span data-stu-id="2e859-129">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="2e859-130">configManager</span><span class="sxs-lookup"><span data-stu-id="2e859-130">configManager</span></span>|<span data-ttu-id="2e859-131">255</span><span class="sxs-lookup"><span data-stu-id="2e859-131">255</span></span>|<span data-ttu-id="2e859-132">Gerenciado pelo Gerenciador de configuração</span><span class="sxs-lookup"><span data-stu-id="2e859-132">Managed by Config Manager</span></span>|





