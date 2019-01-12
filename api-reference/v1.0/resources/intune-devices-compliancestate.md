---
title: tipo de enum complianceState
description: Estado de conformidade.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5a4f4c359665eb1a0087f64802b5e7c829002fd6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940194"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="d59b6-103">tipo de enum complianceState</span><span class="sxs-lookup"><span data-stu-id="d59b6-103">complianceState enum type</span></span>

> <span data-ttu-id="d59b6-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d59b6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d59b6-105">Estado de conformidade.</span><span class="sxs-lookup"><span data-stu-id="d59b6-105">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="d59b6-106">Membros</span><span class="sxs-lookup"><span data-stu-id="d59b6-106">Members</span></span>
|<span data-ttu-id="d59b6-107">Membro</span><span class="sxs-lookup"><span data-stu-id="d59b6-107">Member</span></span>|<span data-ttu-id="d59b6-108">Valor</span><span class="sxs-lookup"><span data-stu-id="d59b6-108">Value</span></span>|<span data-ttu-id="d59b6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d59b6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d59b6-110">unknown</span><span class="sxs-lookup"><span data-stu-id="d59b6-110">unknown</span></span>|<span data-ttu-id="d59b6-111">0</span><span class="sxs-lookup"><span data-stu-id="d59b6-111">0</span></span>|<span data-ttu-id="d59b6-112">Desconhecido.</span><span class="sxs-lookup"><span data-stu-id="d59b6-112">Unknown.</span></span>|
|<span data-ttu-id="d59b6-113">compatível com</span><span class="sxs-lookup"><span data-stu-id="d59b6-113">compliant</span></span>|<span data-ttu-id="d59b6-114">1</span><span class="sxs-lookup"><span data-stu-id="d59b6-114">1</span></span>|<span data-ttu-id="d59b6-115">Compatível com.</span><span class="sxs-lookup"><span data-stu-id="d59b6-115">Compliant.</span></span>|
|<span data-ttu-id="d59b6-116">fora de conformidade</span><span class="sxs-lookup"><span data-stu-id="d59b6-116">noncompliant</span></span>|<span data-ttu-id="d59b6-117">2</span><span class="sxs-lookup"><span data-stu-id="d59b6-117">2</span></span>|<span data-ttu-id="d59b6-118">Dispositivo não está em conformidade e seja bloqueado para recursos corporativos.</span><span class="sxs-lookup"><span data-stu-id="d59b6-118">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="d59b6-119">conflito</span><span class="sxs-lookup"><span data-stu-id="d59b6-119">conflict</span></span>|<span data-ttu-id="d59b6-120">3</span><span class="sxs-lookup"><span data-stu-id="d59b6-120">3</span></span>|<span data-ttu-id="d59b6-121">Conflito com outras regras.</span><span class="sxs-lookup"><span data-stu-id="d59b6-121">Conflict with other rules.</span></span>|
|<span data-ttu-id="d59b6-122">erro</span><span class="sxs-lookup"><span data-stu-id="d59b6-122">error</span></span>|<span data-ttu-id="d59b6-123">4</span><span class="sxs-lookup"><span data-stu-id="d59b6-123">4</span></span>|<span data-ttu-id="d59b6-124">Erro</span><span class="sxs-lookup"><span data-stu-id="d59b6-124">Error.</span></span>|
|<span data-ttu-id="d59b6-125">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="d59b6-125">inGracePeriod</span></span>|<span data-ttu-id="d59b6-126">254</span><span class="sxs-lookup"><span data-stu-id="d59b6-126">254</span></span>|<span data-ttu-id="d59b6-127">Dispositivo não está em conformidade, mas ainda tem acesso aos recursos corporativos</span><span class="sxs-lookup"><span data-stu-id="d59b6-127">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="d59b6-128">configManager</span><span class="sxs-lookup"><span data-stu-id="d59b6-128">configManager</span></span>|<span data-ttu-id="d59b6-129">255</span><span class="sxs-lookup"><span data-stu-id="d59b6-129">255</span></span>|<span data-ttu-id="d59b6-130">Gerenciado pelo Gerenciador de configuração</span><span class="sxs-lookup"><span data-stu-id="d59b6-130">Managed by Config Manager</span></span>|



