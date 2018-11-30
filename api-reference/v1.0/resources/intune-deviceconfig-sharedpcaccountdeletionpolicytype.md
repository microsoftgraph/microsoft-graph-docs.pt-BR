---
title: tipo de enum sharedPCAccountDeletionPolicyType
description: Valores possíveis para quando as contas são excluídas em um PC compartilhado.
ms.openlocfilehash: 48d36881646bce344d99bc3d1a15a2679ddeb11d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005097"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="bf6de-103">tipo de enum sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="bf6de-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="bf6de-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bf6de-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bf6de-105">Valores possíveis para quando as contas são excluídas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="bf6de-105">Possible values for when accounts are deleted on a shared PC.</span></span>
## <a name="members"></a><span data-ttu-id="bf6de-106">Membros</span><span class="sxs-lookup"><span data-stu-id="bf6de-106">Members</span></span>
|<span data-ttu-id="bf6de-107">Membro</span><span class="sxs-lookup"><span data-stu-id="bf6de-107">Member</span></span>|<span data-ttu-id="bf6de-108">Valor</span><span class="sxs-lookup"><span data-stu-id="bf6de-108">Value</span></span>|<span data-ttu-id="bf6de-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf6de-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf6de-110">imediata</span><span class="sxs-lookup"><span data-stu-id="bf6de-110">immediate</span></span>|<span data-ttu-id="bf6de-111">0</span><span class="sxs-lookup"><span data-stu-id="bf6de-111">0</span></span>|<span data-ttu-id="bf6de-112">Exclua imediatamente.</span><span class="sxs-lookup"><span data-stu-id="bf6de-112">Delete immediately.</span></span>|
|<span data-ttu-id="bf6de-113">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="bf6de-113">diskSpaceThreshold</span></span>|<span data-ttu-id="bf6de-114">1</span><span class="sxs-lookup"><span data-stu-id="bf6de-114">1</span></span>|<span data-ttu-id="bf6de-115">Exclua cada limite de espaço em disco.</span><span class="sxs-lookup"><span data-stu-id="bf6de-115">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="bf6de-116">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="bf6de-116">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="bf6de-117">2</span><span class="sxs-lookup"><span data-stu-id="bf6de-117">2</span></span>|<span data-ttu-id="bf6de-118">Exclua cada limite de espaço em disco ou o limite inativa.</span><span class="sxs-lookup"><span data-stu-id="bf6de-118">Delete at disk space threshold or inactive threshold.</span></span>|



