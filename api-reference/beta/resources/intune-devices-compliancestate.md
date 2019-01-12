---
title: tipo de enum complianceState
description: Estado de conformidade.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8936d2116a3aaa8e77905174b46a3997c317cfda
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968712"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="3f3c6-103">tipo de enum complianceState</span><span class="sxs-lookup"><span data-stu-id="3f3c6-103">complianceState enum type</span></span>

> <span data-ttu-id="3f3c6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3f3c6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3f3c6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3f3c6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3f3c6-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3f3c6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3f3c6-107">Estado de conformidade.</span><span class="sxs-lookup"><span data-stu-id="3f3c6-107">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="3f3c6-108">Membros</span><span class="sxs-lookup"><span data-stu-id="3f3c6-108">Members</span></span>
|<span data-ttu-id="3f3c6-109">Membro</span><span class="sxs-lookup"><span data-stu-id="3f3c6-109">Member</span></span>|<span data-ttu-id="3f3c6-110">Valor</span><span class="sxs-lookup"><span data-stu-id="3f3c6-110">Value</span></span>|<span data-ttu-id="3f3c6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f3c6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f3c6-112">unknown</span><span class="sxs-lookup"><span data-stu-id="3f3c6-112">unknown</span></span>|<span data-ttu-id="3f3c6-113">0</span><span class="sxs-lookup"><span data-stu-id="3f3c6-113">0</span></span>|<span data-ttu-id="3f3c6-114">Desconhecido.</span><span class="sxs-lookup"><span data-stu-id="3f3c6-114">Unknown.</span></span>|
|<span data-ttu-id="3f3c6-115">compatível com</span><span class="sxs-lookup"><span data-stu-id="3f3c6-115">compliant</span></span>|<span data-ttu-id="3f3c6-116">1</span><span class="sxs-lookup"><span data-stu-id="3f3c6-116">1</span></span>|<span data-ttu-id="3f3c6-117">Compatível com.</span><span class="sxs-lookup"><span data-stu-id="3f3c6-117">Compliant.</span></span>|
|<span data-ttu-id="3f3c6-118">fora de conformidade</span><span class="sxs-lookup"><span data-stu-id="3f3c6-118">noncompliant</span></span>|<span data-ttu-id="3f3c6-119">2</span><span class="sxs-lookup"><span data-stu-id="3f3c6-119">2</span></span>|<span data-ttu-id="3f3c6-120">Dispositivo não está em conformidade e seja bloqueado para recursos corporativos.</span><span class="sxs-lookup"><span data-stu-id="3f3c6-120">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="3f3c6-121">conflito</span><span class="sxs-lookup"><span data-stu-id="3f3c6-121">conflict</span></span>|<span data-ttu-id="3f3c6-122">3</span><span class="sxs-lookup"><span data-stu-id="3f3c6-122">3</span></span>|<span data-ttu-id="3f3c6-123">Conflito com outras regras.</span><span class="sxs-lookup"><span data-stu-id="3f3c6-123">Conflict with other rules.</span></span>|
|<span data-ttu-id="3f3c6-124">erro</span><span class="sxs-lookup"><span data-stu-id="3f3c6-124">error</span></span>|<span data-ttu-id="3f3c6-125">4</span><span class="sxs-lookup"><span data-stu-id="3f3c6-125">4</span></span>|<span data-ttu-id="3f3c6-126">Erro</span><span class="sxs-lookup"><span data-stu-id="3f3c6-126">Error.</span></span>|
|<span data-ttu-id="3f3c6-127">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="3f3c6-127">inGracePeriod</span></span>|<span data-ttu-id="3f3c6-128">254</span><span class="sxs-lookup"><span data-stu-id="3f3c6-128">254</span></span>|<span data-ttu-id="3f3c6-129">Dispositivo não está em conformidade, mas ainda tem acesso aos recursos corporativos</span><span class="sxs-lookup"><span data-stu-id="3f3c6-129">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="3f3c6-130">configManager</span><span class="sxs-lookup"><span data-stu-id="3f3c6-130">configManager</span></span>|<span data-ttu-id="3f3c6-131">255</span><span class="sxs-lookup"><span data-stu-id="3f3c6-131">255</span></span>|<span data-ttu-id="3f3c6-132">Gerenciado pelo Gerenciador de configuração</span><span class="sxs-lookup"><span data-stu-id="3f3c6-132">Managed by Config Manager</span></span>|





