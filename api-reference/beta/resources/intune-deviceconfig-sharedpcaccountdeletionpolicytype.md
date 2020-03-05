---
title: tipo de enumeração sharedPCAccountDeletionPolicyType
description: Valores possíveis para quando as contas são excluídas em um computador compartilhado.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f843aaf9ace8f41aa83b34993a2229cac91877f1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525863"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="a0a13-103">tipo de enumeração sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="a0a13-103">sharedPCAccountDeletionPolicyType enum type</span></span>

<span data-ttu-id="a0a13-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a0a13-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a0a13-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a0a13-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0a13-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a0a13-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0a13-107">Valores possíveis para quando as contas são excluídas em um computador compartilhado.</span><span class="sxs-lookup"><span data-stu-id="a0a13-107">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="a0a13-108">Membros</span><span class="sxs-lookup"><span data-stu-id="a0a13-108">Members</span></span>
|<span data-ttu-id="a0a13-109">Membro</span><span class="sxs-lookup"><span data-stu-id="a0a13-109">Member</span></span>|<span data-ttu-id="a0a13-110">Valor</span><span class="sxs-lookup"><span data-stu-id="a0a13-110">Value</span></span>|<span data-ttu-id="a0a13-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0a13-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0a13-112">imediato</span><span class="sxs-lookup"><span data-stu-id="a0a13-112">immediate</span></span>|<span data-ttu-id="a0a13-113">,0</span><span class="sxs-lookup"><span data-stu-id="a0a13-113">0</span></span>|<span data-ttu-id="a0a13-114">Excluir imediatamente.</span><span class="sxs-lookup"><span data-stu-id="a0a13-114">Delete immediately.</span></span>|
|<span data-ttu-id="a0a13-115">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="a0a13-115">diskSpaceThreshold</span></span>|<span data-ttu-id="a0a13-116">1 </span><span class="sxs-lookup"><span data-stu-id="a0a13-116">1</span></span>|<span data-ttu-id="a0a13-117">Excluir no limite de espaço em disco.</span><span class="sxs-lookup"><span data-stu-id="a0a13-117">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="a0a13-118">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="a0a13-118">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="a0a13-119">2 </span><span class="sxs-lookup"><span data-stu-id="a0a13-119">2</span></span>|<span data-ttu-id="a0a13-120">Excluir no limite de espaço em disco ou limite inativo.</span><span class="sxs-lookup"><span data-stu-id="a0a13-120">Delete at disk space threshold or inactive threshold.</span></span>|



