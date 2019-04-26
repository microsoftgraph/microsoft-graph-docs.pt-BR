---
title: tipo de enumeração compliancestate
description: Estado de conformidade.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8c462df866b3c711bf4738c70ad4a1b0d68ceeb4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549122"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="bcee7-103">tipo de enumeração compliancestate</span><span class="sxs-lookup"><span data-stu-id="bcee7-103">complianceState enum type</span></span>

> <span data-ttu-id="bcee7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bcee7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bcee7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bcee7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bcee7-106">Estado de conformidade.</span><span class="sxs-lookup"><span data-stu-id="bcee7-106">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="bcee7-107">Membros</span><span class="sxs-lookup"><span data-stu-id="bcee7-107">Members</span></span>
|<span data-ttu-id="bcee7-108">Membro</span><span class="sxs-lookup"><span data-stu-id="bcee7-108">Member</span></span>|<span data-ttu-id="bcee7-109">Valor</span><span class="sxs-lookup"><span data-stu-id="bcee7-109">Value</span></span>|<span data-ttu-id="bcee7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bcee7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcee7-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="bcee7-111">unknown</span></span>|<span data-ttu-id="bcee7-112">,0</span><span class="sxs-lookup"><span data-stu-id="bcee7-112">0</span></span>|<span data-ttu-id="bcee7-113">Unknown.</span><span class="sxs-lookup"><span data-stu-id="bcee7-113">Unknown.</span></span>|
|<span data-ttu-id="bcee7-114">com</span><span class="sxs-lookup"><span data-stu-id="bcee7-114">compliant</span></span>|<span data-ttu-id="bcee7-115">1 </span><span class="sxs-lookup"><span data-stu-id="bcee7-115">1</span></span>|<span data-ttu-id="bcee7-116">Com.</span><span class="sxs-lookup"><span data-stu-id="bcee7-116">Compliant.</span></span>|
|<span data-ttu-id="bcee7-117">incompatível</span><span class="sxs-lookup"><span data-stu-id="bcee7-117">noncompliant</span></span>|<span data-ttu-id="bcee7-118">2 </span><span class="sxs-lookup"><span data-stu-id="bcee7-118">2</span></span>|<span data-ttu-id="bcee7-119">O dispositivo não está em conformidade e é bloqueado de recursos corporativos.</span><span class="sxs-lookup"><span data-stu-id="bcee7-119">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="bcee7-120">apresentar</span><span class="sxs-lookup"><span data-stu-id="bcee7-120">conflict</span></span>|<span data-ttu-id="bcee7-121">3 </span><span class="sxs-lookup"><span data-stu-id="bcee7-121">3</span></span>|<span data-ttu-id="bcee7-122">Conflito com outras regras.</span><span class="sxs-lookup"><span data-stu-id="bcee7-122">Conflict with other rules.</span></span>|
|<span data-ttu-id="bcee7-123">erro</span><span class="sxs-lookup"><span data-stu-id="bcee7-123">error</span></span>|<span data-ttu-id="bcee7-124">4 </span><span class="sxs-lookup"><span data-stu-id="bcee7-124">4</span></span>|<span data-ttu-id="bcee7-125">Erro</span><span class="sxs-lookup"><span data-stu-id="bcee7-125">Error.</span></span>|
|<span data-ttu-id="bcee7-126">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="bcee7-126">inGracePeriod</span></span>|<span data-ttu-id="bcee7-127">254</span><span class="sxs-lookup"><span data-stu-id="bcee7-127">254</span></span>|<span data-ttu-id="bcee7-128">O dispositivo não está em conformidade, mas ainda tem acesso aos recursos corporativos</span><span class="sxs-lookup"><span data-stu-id="bcee7-128">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="bcee7-129">configmanager</span><span class="sxs-lookup"><span data-stu-id="bcee7-129">configManager</span></span>|<span data-ttu-id="bcee7-130">255</span><span class="sxs-lookup"><span data-stu-id="bcee7-130">255</span></span>|<span data-ttu-id="bcee7-131">Gerenciado pelo Gerenciador de configuração</span><span class="sxs-lookup"><span data-stu-id="bcee7-131">Managed by Config Manager</span></span>|





