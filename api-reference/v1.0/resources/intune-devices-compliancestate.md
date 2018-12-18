---
title: tipo de enum complianceState
description: Estado de conformidade.
author: tfitzmac
ms.openlocfilehash: 3045685518f1c7718f9a5f46cd10e0add6fe05b3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330272"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="4d231-103">tipo de enum complianceState</span><span class="sxs-lookup"><span data-stu-id="4d231-103">complianceState enum type</span></span>

> <span data-ttu-id="4d231-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4d231-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4d231-105">Estado de conformidade.</span><span class="sxs-lookup"><span data-stu-id="4d231-105">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="4d231-106">Membros</span><span class="sxs-lookup"><span data-stu-id="4d231-106">Members</span></span>
|<span data-ttu-id="4d231-107">Membro</span><span class="sxs-lookup"><span data-stu-id="4d231-107">Member</span></span>|<span data-ttu-id="4d231-108">Valor</span><span class="sxs-lookup"><span data-stu-id="4d231-108">Value</span></span>|<span data-ttu-id="4d231-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d231-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d231-110">unknown</span><span class="sxs-lookup"><span data-stu-id="4d231-110">unknown</span></span>|<span data-ttu-id="4d231-111">0</span><span class="sxs-lookup"><span data-stu-id="4d231-111">0</span></span>|<span data-ttu-id="4d231-112">Desconhecido.</span><span class="sxs-lookup"><span data-stu-id="4d231-112">Unknown.</span></span>|
|<span data-ttu-id="4d231-113">compatível com</span><span class="sxs-lookup"><span data-stu-id="4d231-113">compliant</span></span>|<span data-ttu-id="4d231-114">1</span><span class="sxs-lookup"><span data-stu-id="4d231-114">1</span></span>|<span data-ttu-id="4d231-115">Compatível com.</span><span class="sxs-lookup"><span data-stu-id="4d231-115">Compliant.</span></span>|
|<span data-ttu-id="4d231-116">fora de conformidade</span><span class="sxs-lookup"><span data-stu-id="4d231-116">noncompliant</span></span>|<span data-ttu-id="4d231-117">2</span><span class="sxs-lookup"><span data-stu-id="4d231-117">2</span></span>|<span data-ttu-id="4d231-118">Dispositivo não está em conformidade e seja bloqueado para recursos corporativos.</span><span class="sxs-lookup"><span data-stu-id="4d231-118">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="4d231-119">conflito</span><span class="sxs-lookup"><span data-stu-id="4d231-119">conflict</span></span>|<span data-ttu-id="4d231-120">3</span><span class="sxs-lookup"><span data-stu-id="4d231-120">3</span></span>|<span data-ttu-id="4d231-121">Conflito com outras regras.</span><span class="sxs-lookup"><span data-stu-id="4d231-121">Conflict with other rules.</span></span>|
|<span data-ttu-id="4d231-122">erro</span><span class="sxs-lookup"><span data-stu-id="4d231-122">error</span></span>|<span data-ttu-id="4d231-123">4</span><span class="sxs-lookup"><span data-stu-id="4d231-123">4</span></span>|<span data-ttu-id="4d231-124">Erro</span><span class="sxs-lookup"><span data-stu-id="4d231-124">Error.</span></span>|
|<span data-ttu-id="4d231-125">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="4d231-125">inGracePeriod</span></span>|<span data-ttu-id="4d231-126">254</span><span class="sxs-lookup"><span data-stu-id="4d231-126">254</span></span>|<span data-ttu-id="4d231-127">Dispositivo não está em conformidade, mas ainda tem acesso aos recursos corporativos</span><span class="sxs-lookup"><span data-stu-id="4d231-127">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="4d231-128">configManager</span><span class="sxs-lookup"><span data-stu-id="4d231-128">configManager</span></span>|<span data-ttu-id="4d231-129">255</span><span class="sxs-lookup"><span data-stu-id="4d231-129">255</span></span>|<span data-ttu-id="4d231-130">Gerenciado pelo Gerenciador de configuração</span><span class="sxs-lookup"><span data-stu-id="4d231-130">Managed by Config Manager</span></span>|



