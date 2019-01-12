---
title: tipo de enum sharedPCAccountDeletionPolicyType
description: Valores possíveis para quando as contas são excluídas em um PC compartilhado.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5dc216d20becdc233bd1664250a958aa7208f1c2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937625"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="2f42a-103">tipo de enum sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="2f42a-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="2f42a-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2f42a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2f42a-105">Valores possíveis para quando as contas são excluídas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="2f42a-105">Possible values for when accounts are deleted on a shared PC.</span></span>
## <a name="members"></a><span data-ttu-id="2f42a-106">Membros</span><span class="sxs-lookup"><span data-stu-id="2f42a-106">Members</span></span>
|<span data-ttu-id="2f42a-107">Membro</span><span class="sxs-lookup"><span data-stu-id="2f42a-107">Member</span></span>|<span data-ttu-id="2f42a-108">Valor</span><span class="sxs-lookup"><span data-stu-id="2f42a-108">Value</span></span>|<span data-ttu-id="2f42a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f42a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f42a-110">imediata</span><span class="sxs-lookup"><span data-stu-id="2f42a-110">immediate</span></span>|<span data-ttu-id="2f42a-111">0</span><span class="sxs-lookup"><span data-stu-id="2f42a-111">0</span></span>|<span data-ttu-id="2f42a-112">Exclua imediatamente.</span><span class="sxs-lookup"><span data-stu-id="2f42a-112">Delete immediately.</span></span>|
|<span data-ttu-id="2f42a-113">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="2f42a-113">diskSpaceThreshold</span></span>|<span data-ttu-id="2f42a-114">1</span><span class="sxs-lookup"><span data-stu-id="2f42a-114">1</span></span>|<span data-ttu-id="2f42a-115">Exclua cada limite de espaço em disco.</span><span class="sxs-lookup"><span data-stu-id="2f42a-115">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="2f42a-116">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="2f42a-116">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="2f42a-117">2</span><span class="sxs-lookup"><span data-stu-id="2f42a-117">2</span></span>|<span data-ttu-id="2f42a-118">Exclua cada limite de espaço em disco ou o limite inativa.</span><span class="sxs-lookup"><span data-stu-id="2f42a-118">Delete at disk space threshold or inactive threshold.</span></span>|



