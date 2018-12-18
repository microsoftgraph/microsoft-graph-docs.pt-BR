---
title: tipo de enum complianceState
description: Estado de conformidade.
author: tfitzmac
ms.openlocfilehash: 3fa0548c2a67aa5def5f859014f52e97bdda815b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321228"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="7c608-103">tipo de enum complianceState</span><span class="sxs-lookup"><span data-stu-id="7c608-103">complianceState enum type</span></span>

> <span data-ttu-id="7c608-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7c608-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7c608-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7c608-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7c608-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7c608-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7c608-107">Estado de conformidade.</span><span class="sxs-lookup"><span data-stu-id="7c608-107">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="7c608-108">Membros</span><span class="sxs-lookup"><span data-stu-id="7c608-108">Members</span></span>
|<span data-ttu-id="7c608-109">Membro</span><span class="sxs-lookup"><span data-stu-id="7c608-109">Member</span></span>|<span data-ttu-id="7c608-110">Valor</span><span class="sxs-lookup"><span data-stu-id="7c608-110">Value</span></span>|<span data-ttu-id="7c608-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c608-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c608-112">unknown</span><span class="sxs-lookup"><span data-stu-id="7c608-112">unknown</span></span>|<span data-ttu-id="7c608-113">0</span><span class="sxs-lookup"><span data-stu-id="7c608-113">0</span></span>|<span data-ttu-id="7c608-114">Desconhecido.</span><span class="sxs-lookup"><span data-stu-id="7c608-114">Unknown.</span></span>|
|<span data-ttu-id="7c608-115">compatível com</span><span class="sxs-lookup"><span data-stu-id="7c608-115">compliant</span></span>|<span data-ttu-id="7c608-116">1</span><span class="sxs-lookup"><span data-stu-id="7c608-116">1</span></span>|<span data-ttu-id="7c608-117">Compatível com.</span><span class="sxs-lookup"><span data-stu-id="7c608-117">Compliant.</span></span>|
|<span data-ttu-id="7c608-118">fora de conformidade</span><span class="sxs-lookup"><span data-stu-id="7c608-118">noncompliant</span></span>|<span data-ttu-id="7c608-119">2</span><span class="sxs-lookup"><span data-stu-id="7c608-119">2</span></span>|<span data-ttu-id="7c608-120">Dispositivo não está em conformidade e seja bloqueado para recursos corporativos.</span><span class="sxs-lookup"><span data-stu-id="7c608-120">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="7c608-121">conflito</span><span class="sxs-lookup"><span data-stu-id="7c608-121">conflict</span></span>|<span data-ttu-id="7c608-122">3</span><span class="sxs-lookup"><span data-stu-id="7c608-122">3</span></span>|<span data-ttu-id="7c608-123">Conflito com outras regras.</span><span class="sxs-lookup"><span data-stu-id="7c608-123">Conflict with other rules.</span></span>|
|<span data-ttu-id="7c608-124">erro</span><span class="sxs-lookup"><span data-stu-id="7c608-124">error</span></span>|<span data-ttu-id="7c608-125">4</span><span class="sxs-lookup"><span data-stu-id="7c608-125">4</span></span>|<span data-ttu-id="7c608-126">Erro</span><span class="sxs-lookup"><span data-stu-id="7c608-126">Error.</span></span>|
|<span data-ttu-id="7c608-127">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="7c608-127">inGracePeriod</span></span>|<span data-ttu-id="7c608-128">254</span><span class="sxs-lookup"><span data-stu-id="7c608-128">254</span></span>|<span data-ttu-id="7c608-129">Dispositivo não está em conformidade, mas ainda tem acesso aos recursos corporativos</span><span class="sxs-lookup"><span data-stu-id="7c608-129">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="7c608-130">configManager</span><span class="sxs-lookup"><span data-stu-id="7c608-130">configManager</span></span>|<span data-ttu-id="7c608-131">255</span><span class="sxs-lookup"><span data-stu-id="7c608-131">255</span></span>|<span data-ttu-id="7c608-132">Gerenciado pelo Gerenciador de configuração</span><span class="sxs-lookup"><span data-stu-id="7c608-132">Managed by Config Manager</span></span>|





