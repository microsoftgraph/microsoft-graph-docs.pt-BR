---
title: tipo de enumeração sharedPCAccountDeletionPolicyType
description: Valores possíveis para quando as contas são excluídas em um computador compartilhado.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 539591836b9771b1b00288c33f08c3db754f322d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443347"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="72e6c-103">tipo de enumeração sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="72e6c-103">sharedPCAccountDeletionPolicyType enum type</span></span>

<span data-ttu-id="72e6c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72e6c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72e6c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="72e6c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72e6c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="72e6c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72e6c-107">Valores possíveis para quando as contas são excluídas em um computador compartilhado.</span><span class="sxs-lookup"><span data-stu-id="72e6c-107">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="72e6c-108">Membros</span><span class="sxs-lookup"><span data-stu-id="72e6c-108">Members</span></span>
|<span data-ttu-id="72e6c-109">Membro</span><span class="sxs-lookup"><span data-stu-id="72e6c-109">Member</span></span>|<span data-ttu-id="72e6c-110">Valor</span><span class="sxs-lookup"><span data-stu-id="72e6c-110">Value</span></span>|<span data-ttu-id="72e6c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="72e6c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72e6c-112">imediato</span><span class="sxs-lookup"><span data-stu-id="72e6c-112">immediate</span></span>|<span data-ttu-id="72e6c-113">,0</span><span class="sxs-lookup"><span data-stu-id="72e6c-113">0</span></span>|<span data-ttu-id="72e6c-114">Excluir imediatamente.</span><span class="sxs-lookup"><span data-stu-id="72e6c-114">Delete immediately.</span></span>|
|<span data-ttu-id="72e6c-115">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="72e6c-115">diskSpaceThreshold</span></span>|<span data-ttu-id="72e6c-116">1</span><span class="sxs-lookup"><span data-stu-id="72e6c-116">1</span></span>|<span data-ttu-id="72e6c-117">Excluir no limite de espaço em disco.</span><span class="sxs-lookup"><span data-stu-id="72e6c-117">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="72e6c-118">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="72e6c-118">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="72e6c-119">duas</span><span class="sxs-lookup"><span data-stu-id="72e6c-119">2</span></span>|<span data-ttu-id="72e6c-120">Excluir no limite de espaço em disco ou limite inativo.</span><span class="sxs-lookup"><span data-stu-id="72e6c-120">Delete at disk space threshold or inactive threshold.</span></span>|



