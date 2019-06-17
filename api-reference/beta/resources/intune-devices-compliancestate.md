---
title: tipo de enumeração compliancestate
description: Estado de conformidade.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 83f39e4c795d57b6bb5aa5633ed481963419e041
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983285"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="79a46-103">tipo de enumeração compliancestate</span><span class="sxs-lookup"><span data-stu-id="79a46-103">complianceState enum type</span></span>

> <span data-ttu-id="79a46-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="79a46-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79a46-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="79a46-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79a46-106">Estado de conformidade.</span><span class="sxs-lookup"><span data-stu-id="79a46-106">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="79a46-107">Membros</span><span class="sxs-lookup"><span data-stu-id="79a46-107">Members</span></span>
|<span data-ttu-id="79a46-108">Membro</span><span class="sxs-lookup"><span data-stu-id="79a46-108">Member</span></span>|<span data-ttu-id="79a46-109">Valor</span><span class="sxs-lookup"><span data-stu-id="79a46-109">Value</span></span>|<span data-ttu-id="79a46-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="79a46-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79a46-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="79a46-111">unknown</span></span>|<span data-ttu-id="79a46-112">,0</span><span class="sxs-lookup"><span data-stu-id="79a46-112">0</span></span>|<span data-ttu-id="79a46-113">Unknown.</span><span class="sxs-lookup"><span data-stu-id="79a46-113">Unknown.</span></span>|
|<span data-ttu-id="79a46-114">com</span><span class="sxs-lookup"><span data-stu-id="79a46-114">compliant</span></span>|<span data-ttu-id="79a46-115">1</span><span class="sxs-lookup"><span data-stu-id="79a46-115">1</span></span>|<span data-ttu-id="79a46-116">Com.</span><span class="sxs-lookup"><span data-stu-id="79a46-116">Compliant.</span></span>|
|<span data-ttu-id="79a46-117">incompatível</span><span class="sxs-lookup"><span data-stu-id="79a46-117">noncompliant</span></span>|<span data-ttu-id="79a46-118">duas</span><span class="sxs-lookup"><span data-stu-id="79a46-118">2</span></span>|<span data-ttu-id="79a46-119">O dispositivo não está em conformidade e é bloqueado de recursos corporativos.</span><span class="sxs-lookup"><span data-stu-id="79a46-119">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="79a46-120">apresentar</span><span class="sxs-lookup"><span data-stu-id="79a46-120">conflict</span></span>|<span data-ttu-id="79a46-121">3D</span><span class="sxs-lookup"><span data-stu-id="79a46-121">3</span></span>|<span data-ttu-id="79a46-122">Conflito com outras regras.</span><span class="sxs-lookup"><span data-stu-id="79a46-122">Conflict with other rules.</span></span>|
|<span data-ttu-id="79a46-123">erro</span><span class="sxs-lookup"><span data-stu-id="79a46-123">error</span></span>|<span data-ttu-id="79a46-124">quatro</span><span class="sxs-lookup"><span data-stu-id="79a46-124">4</span></span>|<span data-ttu-id="79a46-125">Erro</span><span class="sxs-lookup"><span data-stu-id="79a46-125">Error.</span></span>|
|<span data-ttu-id="79a46-126">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="79a46-126">inGracePeriod</span></span>|<span data-ttu-id="79a46-127">254</span><span class="sxs-lookup"><span data-stu-id="79a46-127">254</span></span>|<span data-ttu-id="79a46-128">O dispositivo não está em conformidade, mas ainda tem acesso aos recursos corporativos</span><span class="sxs-lookup"><span data-stu-id="79a46-128">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="79a46-129">configmanager</span><span class="sxs-lookup"><span data-stu-id="79a46-129">configManager</span></span>|<span data-ttu-id="79a46-130">255</span><span class="sxs-lookup"><span data-stu-id="79a46-130">255</span></span>|<span data-ttu-id="79a46-131">Gerenciado pelo Gerenciador de configuração</span><span class="sxs-lookup"><span data-stu-id="79a46-131">Managed by Config Manager</span></span>|





