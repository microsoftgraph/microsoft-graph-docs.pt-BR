---
title: tipo de enumeração compliancestate
description: Estado de conformidade.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 20890001aee15a56d5338964b931047033cf4a72
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030881"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="c3a5b-103">tipo de enumeração compliancestate</span><span class="sxs-lookup"><span data-stu-id="c3a5b-103">complianceState enum type</span></span>

> <span data-ttu-id="c3a5b-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c3a5b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3a5b-105">Estado de conformidade.</span><span class="sxs-lookup"><span data-stu-id="c3a5b-105">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="c3a5b-106">Membros</span><span class="sxs-lookup"><span data-stu-id="c3a5b-106">Members</span></span>
|<span data-ttu-id="c3a5b-107">Membro</span><span class="sxs-lookup"><span data-stu-id="c3a5b-107">Member</span></span>|<span data-ttu-id="c3a5b-108">Valor</span><span class="sxs-lookup"><span data-stu-id="c3a5b-108">Value</span></span>|<span data-ttu-id="c3a5b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3a5b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3a5b-110">desconhecido</span><span class="sxs-lookup"><span data-stu-id="c3a5b-110">unknown</span></span>|<span data-ttu-id="c3a5b-111">,0</span><span class="sxs-lookup"><span data-stu-id="c3a5b-111">0</span></span>|<span data-ttu-id="c3a5b-112">Unknown.</span><span class="sxs-lookup"><span data-stu-id="c3a5b-112">Unknown.</span></span>|
|<span data-ttu-id="c3a5b-113">com</span><span class="sxs-lookup"><span data-stu-id="c3a5b-113">compliant</span></span>|<span data-ttu-id="c3a5b-114">1</span><span class="sxs-lookup"><span data-stu-id="c3a5b-114">1</span></span>|<span data-ttu-id="c3a5b-115">Com.</span><span class="sxs-lookup"><span data-stu-id="c3a5b-115">Compliant.</span></span>|
|<span data-ttu-id="c3a5b-116">incompatível</span><span class="sxs-lookup"><span data-stu-id="c3a5b-116">noncompliant</span></span>|<span data-ttu-id="c3a5b-117">duas</span><span class="sxs-lookup"><span data-stu-id="c3a5b-117">2</span></span>|<span data-ttu-id="c3a5b-118">O dispositivo não está em conformidade e é bloqueado de recursos corporativos.</span><span class="sxs-lookup"><span data-stu-id="c3a5b-118">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="c3a5b-119">apresentar</span><span class="sxs-lookup"><span data-stu-id="c3a5b-119">conflict</span></span>|<span data-ttu-id="c3a5b-120">3D</span><span class="sxs-lookup"><span data-stu-id="c3a5b-120">3</span></span>|<span data-ttu-id="c3a5b-121">Conflito com outras regras.</span><span class="sxs-lookup"><span data-stu-id="c3a5b-121">Conflict with other rules.</span></span>|
|<span data-ttu-id="c3a5b-122">erro</span><span class="sxs-lookup"><span data-stu-id="c3a5b-122">error</span></span>|<span data-ttu-id="c3a5b-123">quatro</span><span class="sxs-lookup"><span data-stu-id="c3a5b-123">4</span></span>|<span data-ttu-id="c3a5b-124">Erro</span><span class="sxs-lookup"><span data-stu-id="c3a5b-124">Error.</span></span>|
|<span data-ttu-id="c3a5b-125">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="c3a5b-125">inGracePeriod</span></span>|<span data-ttu-id="c3a5b-126">254</span><span class="sxs-lookup"><span data-stu-id="c3a5b-126">254</span></span>|<span data-ttu-id="c3a5b-127">O dispositivo não está em conformidade, mas ainda tem acesso aos recursos corporativos</span><span class="sxs-lookup"><span data-stu-id="c3a5b-127">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="c3a5b-128">configmanager</span><span class="sxs-lookup"><span data-stu-id="c3a5b-128">configManager</span></span>|<span data-ttu-id="c3a5b-129">255</span><span class="sxs-lookup"><span data-stu-id="c3a5b-129">255</span></span>|<span data-ttu-id="c3a5b-130">Gerenciado pelo Gerenciador de configuração</span><span class="sxs-lookup"><span data-stu-id="c3a5b-130">Managed by Config Manager</span></span>|



