---
title: tipo de enum sharedPCAccountDeletionPolicyType
description: Valores possíveis para quando as contas são excluídas em um PC compartilhado.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6a1e3c9e15409e253852b4b896e18181ef1bc391
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884121"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="2262b-103">tipo de enum sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="2262b-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="2262b-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2262b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2262b-105">Valores possíveis para quando as contas são excluídas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="2262b-105">Possible values for when accounts are deleted on a shared PC.</span></span>
## <a name="members"></a><span data-ttu-id="2262b-106">Membros</span><span class="sxs-lookup"><span data-stu-id="2262b-106">Members</span></span>
|<span data-ttu-id="2262b-107">Membro</span><span class="sxs-lookup"><span data-stu-id="2262b-107">Member</span></span>|<span data-ttu-id="2262b-108">Valor</span><span class="sxs-lookup"><span data-stu-id="2262b-108">Value</span></span>|<span data-ttu-id="2262b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2262b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2262b-110">imediata</span><span class="sxs-lookup"><span data-stu-id="2262b-110">immediate</span></span>|<span data-ttu-id="2262b-111">0</span><span class="sxs-lookup"><span data-stu-id="2262b-111">0</span></span>|<span data-ttu-id="2262b-112">Exclua imediatamente.</span><span class="sxs-lookup"><span data-stu-id="2262b-112">Delete immediately.</span></span>|
|<span data-ttu-id="2262b-113">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="2262b-113">diskSpaceThreshold</span></span>|<span data-ttu-id="2262b-114">1</span><span class="sxs-lookup"><span data-stu-id="2262b-114">1</span></span>|<span data-ttu-id="2262b-115">Exclua cada limite de espaço em disco.</span><span class="sxs-lookup"><span data-stu-id="2262b-115">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="2262b-116">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="2262b-116">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="2262b-117">2</span><span class="sxs-lookup"><span data-stu-id="2262b-117">2</span></span>|<span data-ttu-id="2262b-118">Exclua cada limite de espaço em disco ou o limite inativa.</span><span class="sxs-lookup"><span data-stu-id="2262b-118">Delete at disk space threshold or inactive threshold.</span></span>|



