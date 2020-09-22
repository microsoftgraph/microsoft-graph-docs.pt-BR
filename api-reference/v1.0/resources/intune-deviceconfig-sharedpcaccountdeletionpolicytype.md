---
title: tipo de enumeração sharedPCAccountDeletionPolicyType
description: Valores possíveis para quando as contas são excluídas em um computador compartilhado.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b8fb006173b974ac902a99a2257ebbaeb52ea1d0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48066450"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="87b9c-103">tipo de enumeração sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="87b9c-103">sharedPCAccountDeletionPolicyType enum type</span></span>

<span data-ttu-id="87b9c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87b9c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="87b9c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="87b9c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87b9c-106">Valores possíveis para quando as contas são excluídas em um computador compartilhado.</span><span class="sxs-lookup"><span data-stu-id="87b9c-106">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="87b9c-107">Membros</span><span class="sxs-lookup"><span data-stu-id="87b9c-107">Members</span></span>
|<span data-ttu-id="87b9c-108">Membro</span><span class="sxs-lookup"><span data-stu-id="87b9c-108">Member</span></span>|<span data-ttu-id="87b9c-109">Valor</span><span class="sxs-lookup"><span data-stu-id="87b9c-109">Value</span></span>|<span data-ttu-id="87b9c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="87b9c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87b9c-111">imediato</span><span class="sxs-lookup"><span data-stu-id="87b9c-111">immediate</span></span>|<span data-ttu-id="87b9c-112">,0</span><span class="sxs-lookup"><span data-stu-id="87b9c-112">0</span></span>|<span data-ttu-id="87b9c-113">Excluir imediatamente.</span><span class="sxs-lookup"><span data-stu-id="87b9c-113">Delete immediately.</span></span>|
|<span data-ttu-id="87b9c-114">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="87b9c-114">diskSpaceThreshold</span></span>|<span data-ttu-id="87b9c-115">1 </span><span class="sxs-lookup"><span data-stu-id="87b9c-115">1</span></span>|<span data-ttu-id="87b9c-116">Excluir no limite de espaço em disco.</span><span class="sxs-lookup"><span data-stu-id="87b9c-116">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="87b9c-117">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="87b9c-117">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="87b9c-118">2 </span><span class="sxs-lookup"><span data-stu-id="87b9c-118">2</span></span>|<span data-ttu-id="87b9c-119">Excluir no limite de espaço em disco ou limite inativo.</span><span class="sxs-lookup"><span data-stu-id="87b9c-119">Delete at disk space threshold or inactive threshold.</span></span>|









