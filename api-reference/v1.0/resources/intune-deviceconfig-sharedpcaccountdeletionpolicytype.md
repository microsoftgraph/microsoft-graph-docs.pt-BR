---
title: tipo de enum sharedPCAccountDeletionPolicyType
description: Valores possíveis para quando as contas são excluídas em um PC compartilhado.
author: tfitzmac
ms.openlocfilehash: 8789faeeec7772cd6115cae82691c62894446f59
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27300998"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="514da-103">tipo de enum sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="514da-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="514da-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="514da-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="514da-105">Valores possíveis para quando as contas são excluídas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="514da-105">Possible values for when accounts are deleted on a shared PC.</span></span>
## <a name="members"></a><span data-ttu-id="514da-106">Membros</span><span class="sxs-lookup"><span data-stu-id="514da-106">Members</span></span>
|<span data-ttu-id="514da-107">Membro</span><span class="sxs-lookup"><span data-stu-id="514da-107">Member</span></span>|<span data-ttu-id="514da-108">Valor</span><span class="sxs-lookup"><span data-stu-id="514da-108">Value</span></span>|<span data-ttu-id="514da-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="514da-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="514da-110">imediata</span><span class="sxs-lookup"><span data-stu-id="514da-110">immediate</span></span>|<span data-ttu-id="514da-111">0</span><span class="sxs-lookup"><span data-stu-id="514da-111">0</span></span>|<span data-ttu-id="514da-112">Exclua imediatamente.</span><span class="sxs-lookup"><span data-stu-id="514da-112">Delete immediately.</span></span>|
|<span data-ttu-id="514da-113">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="514da-113">diskSpaceThreshold</span></span>|<span data-ttu-id="514da-114">1</span><span class="sxs-lookup"><span data-stu-id="514da-114">1</span></span>|<span data-ttu-id="514da-115">Exclua cada limite de espaço em disco.</span><span class="sxs-lookup"><span data-stu-id="514da-115">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="514da-116">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="514da-116">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="514da-117">2</span><span class="sxs-lookup"><span data-stu-id="514da-117">2</span></span>|<span data-ttu-id="514da-118">Exclua cada limite de espaço em disco ou o limite inativa.</span><span class="sxs-lookup"><span data-stu-id="514da-118">Delete at disk space threshold or inactive threshold.</span></span>|



