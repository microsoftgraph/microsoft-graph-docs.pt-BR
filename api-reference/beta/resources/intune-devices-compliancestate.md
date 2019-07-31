---
title: tipo de enumeração compliancestate
description: Estado de conformidade.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 6fff27abba5bce945b1f8abd74e94e2060114b17
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000015"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="46ddf-103">tipo de enumeração compliancestate</span><span class="sxs-lookup"><span data-stu-id="46ddf-103">complianceState enum type</span></span>

> <span data-ttu-id="46ddf-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="46ddf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46ddf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="46ddf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46ddf-106">Estado de conformidade.</span><span class="sxs-lookup"><span data-stu-id="46ddf-106">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="46ddf-107">Membros</span><span class="sxs-lookup"><span data-stu-id="46ddf-107">Members</span></span>
|<span data-ttu-id="46ddf-108">Membro</span><span class="sxs-lookup"><span data-stu-id="46ddf-108">Member</span></span>|<span data-ttu-id="46ddf-109">Valor</span><span class="sxs-lookup"><span data-stu-id="46ddf-109">Value</span></span>|<span data-ttu-id="46ddf-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="46ddf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46ddf-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="46ddf-111">unknown</span></span>|<span data-ttu-id="46ddf-112">,0</span><span class="sxs-lookup"><span data-stu-id="46ddf-112">0</span></span>|<span data-ttu-id="46ddf-113">Unknown.</span><span class="sxs-lookup"><span data-stu-id="46ddf-113">Unknown.</span></span>|
|<span data-ttu-id="46ddf-114">com</span><span class="sxs-lookup"><span data-stu-id="46ddf-114">compliant</span></span>|<span data-ttu-id="46ddf-115">1</span><span class="sxs-lookup"><span data-stu-id="46ddf-115">1</span></span>|<span data-ttu-id="46ddf-116">Com.</span><span class="sxs-lookup"><span data-stu-id="46ddf-116">Compliant.</span></span>|
|<span data-ttu-id="46ddf-117">incompatível</span><span class="sxs-lookup"><span data-stu-id="46ddf-117">noncompliant</span></span>|<span data-ttu-id="46ddf-118">duas</span><span class="sxs-lookup"><span data-stu-id="46ddf-118">2</span></span>|<span data-ttu-id="46ddf-119">O dispositivo não está em conformidade e é bloqueado de recursos corporativos.</span><span class="sxs-lookup"><span data-stu-id="46ddf-119">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="46ddf-120">apresentar</span><span class="sxs-lookup"><span data-stu-id="46ddf-120">conflict</span></span>|<span data-ttu-id="46ddf-121">3D</span><span class="sxs-lookup"><span data-stu-id="46ddf-121">3</span></span>|<span data-ttu-id="46ddf-122">Conflito com outras regras.</span><span class="sxs-lookup"><span data-stu-id="46ddf-122">Conflict with other rules.</span></span>|
|<span data-ttu-id="46ddf-123">erro</span><span class="sxs-lookup"><span data-stu-id="46ddf-123">error</span></span>|<span data-ttu-id="46ddf-124">quatro</span><span class="sxs-lookup"><span data-stu-id="46ddf-124">4</span></span>|<span data-ttu-id="46ddf-125">Erro</span><span class="sxs-lookup"><span data-stu-id="46ddf-125">Error.</span></span>|
|<span data-ttu-id="46ddf-126">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="46ddf-126">inGracePeriod</span></span>|<span data-ttu-id="46ddf-127">254</span><span class="sxs-lookup"><span data-stu-id="46ddf-127">254</span></span>|<span data-ttu-id="46ddf-128">O dispositivo não está em conformidade, mas ainda tem acesso aos recursos corporativos</span><span class="sxs-lookup"><span data-stu-id="46ddf-128">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="46ddf-129">configmanager</span><span class="sxs-lookup"><span data-stu-id="46ddf-129">configManager</span></span>|<span data-ttu-id="46ddf-130">255</span><span class="sxs-lookup"><span data-stu-id="46ddf-130">255</span></span>|<span data-ttu-id="46ddf-131">Gerenciado pelo Gerenciador de configuração</span><span class="sxs-lookup"><span data-stu-id="46ddf-131">Managed by Config Manager</span></span>|





