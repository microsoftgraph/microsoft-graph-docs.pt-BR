---
title: tipo de enumeração sharedPCAccountDeletionPolicyType
description: Valores possíveis para quando as contas são excluídas em um computador compartilhado.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0c547a59c02e3c4cad9bd8140a2e11ca6e3c84a7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534616"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="92318-103">tipo de enumeração sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="92318-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="92318-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="92318-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92318-105">Valores possíveis para quando as contas são excluídas em um computador compartilhado.</span><span class="sxs-lookup"><span data-stu-id="92318-105">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="92318-106">Membros</span><span class="sxs-lookup"><span data-stu-id="92318-106">Members</span></span>
|<span data-ttu-id="92318-107">Membro</span><span class="sxs-lookup"><span data-stu-id="92318-107">Member</span></span>|<span data-ttu-id="92318-108">Valor</span><span class="sxs-lookup"><span data-stu-id="92318-108">Value</span></span>|<span data-ttu-id="92318-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="92318-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92318-110">imediato</span><span class="sxs-lookup"><span data-stu-id="92318-110">immediate</span></span>|<span data-ttu-id="92318-111">,0</span><span class="sxs-lookup"><span data-stu-id="92318-111">0</span></span>|<span data-ttu-id="92318-112">Excluir imediatamente.</span><span class="sxs-lookup"><span data-stu-id="92318-112">Delete immediately.</span></span>|
|<span data-ttu-id="92318-113">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="92318-113">diskSpaceThreshold</span></span>|<span data-ttu-id="92318-114">1 </span><span class="sxs-lookup"><span data-stu-id="92318-114">1</span></span>|<span data-ttu-id="92318-115">Excluir no limite de espaço em disco.</span><span class="sxs-lookup"><span data-stu-id="92318-115">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="92318-116">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="92318-116">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="92318-117">2 </span><span class="sxs-lookup"><span data-stu-id="92318-117">2</span></span>|<span data-ttu-id="92318-118">Excluir no limite de espaço em disco ou limite inativo.</span><span class="sxs-lookup"><span data-stu-id="92318-118">Delete at disk space threshold or inactive threshold.</span></span>|



