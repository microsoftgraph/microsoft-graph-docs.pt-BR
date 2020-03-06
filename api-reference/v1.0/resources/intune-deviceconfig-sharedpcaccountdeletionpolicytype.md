---
title: tipo de enumeração sharedPCAccountDeletionPolicyType
description: Valores possíveis para quando as contas são excluídas em um computador compartilhado.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4a60f207c36c8c17291d15789f33e391ea8c6d40
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532335"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="180a8-103">tipo de enumeração sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="180a8-103">sharedPCAccountDeletionPolicyType enum type</span></span>

<span data-ttu-id="180a8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="180a8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="180a8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="180a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="180a8-106">Valores possíveis para quando as contas são excluídas em um computador compartilhado.</span><span class="sxs-lookup"><span data-stu-id="180a8-106">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="180a8-107">Membros</span><span class="sxs-lookup"><span data-stu-id="180a8-107">Members</span></span>
|<span data-ttu-id="180a8-108">Membro</span><span class="sxs-lookup"><span data-stu-id="180a8-108">Member</span></span>|<span data-ttu-id="180a8-109">Valor</span><span class="sxs-lookup"><span data-stu-id="180a8-109">Value</span></span>|<span data-ttu-id="180a8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="180a8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="180a8-111">imediato</span><span class="sxs-lookup"><span data-stu-id="180a8-111">immediate</span></span>|<span data-ttu-id="180a8-112">,0</span><span class="sxs-lookup"><span data-stu-id="180a8-112">0</span></span>|<span data-ttu-id="180a8-113">Excluir imediatamente.</span><span class="sxs-lookup"><span data-stu-id="180a8-113">Delete immediately.</span></span>|
|<span data-ttu-id="180a8-114">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="180a8-114">diskSpaceThreshold</span></span>|<span data-ttu-id="180a8-115">1 </span><span class="sxs-lookup"><span data-stu-id="180a8-115">1</span></span>|<span data-ttu-id="180a8-116">Excluir no limite de espaço em disco.</span><span class="sxs-lookup"><span data-stu-id="180a8-116">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="180a8-117">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="180a8-117">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="180a8-118">2 </span><span class="sxs-lookup"><span data-stu-id="180a8-118">2</span></span>|<span data-ttu-id="180a8-119">Excluir no limite de espaço em disco ou limite inativo.</span><span class="sxs-lookup"><span data-stu-id="180a8-119">Delete at disk space threshold or inactive threshold.</span></span>|




