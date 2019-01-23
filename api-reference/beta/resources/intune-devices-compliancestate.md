---
title: tipo de enum complianceState
description: Estado de conformidade.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 04f77da451970a302dbf249e8820aa5a2a8f0ebc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392735"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="16be8-103">tipo de enum complianceState</span><span class="sxs-lookup"><span data-stu-id="16be8-103">complianceState enum type</span></span>

> <span data-ttu-id="16be8-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="16be8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="16be8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="16be8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="16be8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="16be8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16be8-107">Estado de conformidade.</span><span class="sxs-lookup"><span data-stu-id="16be8-107">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="16be8-108">Membros</span><span class="sxs-lookup"><span data-stu-id="16be8-108">Members</span></span>
|<span data-ttu-id="16be8-109">Membro</span><span class="sxs-lookup"><span data-stu-id="16be8-109">Member</span></span>|<span data-ttu-id="16be8-110">Valor</span><span class="sxs-lookup"><span data-stu-id="16be8-110">Value</span></span>|<span data-ttu-id="16be8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="16be8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16be8-112">unknown</span><span class="sxs-lookup"><span data-stu-id="16be8-112">unknown</span></span>|<span data-ttu-id="16be8-113">0</span><span class="sxs-lookup"><span data-stu-id="16be8-113">0</span></span>|<span data-ttu-id="16be8-114">Desconhecido.</span><span class="sxs-lookup"><span data-stu-id="16be8-114">Unknown.</span></span>|
|<span data-ttu-id="16be8-115">compatível com</span><span class="sxs-lookup"><span data-stu-id="16be8-115">compliant</span></span>|<span data-ttu-id="16be8-116">1</span><span class="sxs-lookup"><span data-stu-id="16be8-116">1</span></span>|<span data-ttu-id="16be8-117">Compatível com.</span><span class="sxs-lookup"><span data-stu-id="16be8-117">Compliant.</span></span>|
|<span data-ttu-id="16be8-118">fora de conformidade</span><span class="sxs-lookup"><span data-stu-id="16be8-118">noncompliant</span></span>|<span data-ttu-id="16be8-119">2</span><span class="sxs-lookup"><span data-stu-id="16be8-119">2</span></span>|<span data-ttu-id="16be8-120">Dispositivo não está em conformidade e seja bloqueado para recursos corporativos.</span><span class="sxs-lookup"><span data-stu-id="16be8-120">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="16be8-121">conflito</span><span class="sxs-lookup"><span data-stu-id="16be8-121">conflict</span></span>|<span data-ttu-id="16be8-122">3</span><span class="sxs-lookup"><span data-stu-id="16be8-122">3</span></span>|<span data-ttu-id="16be8-123">Conflito com outras regras.</span><span class="sxs-lookup"><span data-stu-id="16be8-123">Conflict with other rules.</span></span>|
|<span data-ttu-id="16be8-124">erro</span><span class="sxs-lookup"><span data-stu-id="16be8-124">error</span></span>|<span data-ttu-id="16be8-125">4</span><span class="sxs-lookup"><span data-stu-id="16be8-125">4</span></span>|<span data-ttu-id="16be8-126">Erro</span><span class="sxs-lookup"><span data-stu-id="16be8-126">Error.</span></span>|
|<span data-ttu-id="16be8-127">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="16be8-127">inGracePeriod</span></span>|<span data-ttu-id="16be8-128">254</span><span class="sxs-lookup"><span data-stu-id="16be8-128">254</span></span>|<span data-ttu-id="16be8-129">Dispositivo não está em conformidade, mas ainda tem acesso aos recursos corporativos</span><span class="sxs-lookup"><span data-stu-id="16be8-129">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="16be8-130">configManager</span><span class="sxs-lookup"><span data-stu-id="16be8-130">configManager</span></span>|<span data-ttu-id="16be8-131">255</span><span class="sxs-lookup"><span data-stu-id="16be8-131">255</span></span>|<span data-ttu-id="16be8-132">Gerenciado pelo Gerenciador de configuração</span><span class="sxs-lookup"><span data-stu-id="16be8-132">Managed by Config Manager</span></span>|




