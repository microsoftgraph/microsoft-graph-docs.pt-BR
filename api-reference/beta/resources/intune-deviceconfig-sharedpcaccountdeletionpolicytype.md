---
title: tipo de enum sharedPCAccountDeletionPolicyType
description: Valores possíveis para quando as contas são excluídas em um PC compartilhado.
author: tfitzmac
ms.openlocfilehash: 626bc7ee4006639396a7959c4f09bec47c2d7f68
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27335046"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="7e979-103">tipo de enum sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="7e979-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="7e979-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7e979-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7e979-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7e979-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7e979-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7e979-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7e979-107">Valores possíveis para quando as contas são excluídas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="7e979-107">Possible values for when accounts are deleted on a shared PC.</span></span>
## <a name="members"></a><span data-ttu-id="7e979-108">Membros</span><span class="sxs-lookup"><span data-stu-id="7e979-108">Members</span></span>
|<span data-ttu-id="7e979-109">Membro</span><span class="sxs-lookup"><span data-stu-id="7e979-109">Member</span></span>|<span data-ttu-id="7e979-110">Valor</span><span class="sxs-lookup"><span data-stu-id="7e979-110">Value</span></span>|<span data-ttu-id="7e979-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e979-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e979-112">imediata</span><span class="sxs-lookup"><span data-stu-id="7e979-112">immediate</span></span>|<span data-ttu-id="7e979-113">0</span><span class="sxs-lookup"><span data-stu-id="7e979-113">0</span></span>|<span data-ttu-id="7e979-114">Exclua imediatamente.</span><span class="sxs-lookup"><span data-stu-id="7e979-114">Delete immediately.</span></span>|
|<span data-ttu-id="7e979-115">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="7e979-115">diskSpaceThreshold</span></span>|<span data-ttu-id="7e979-116">1</span><span class="sxs-lookup"><span data-stu-id="7e979-116">1</span></span>|<span data-ttu-id="7e979-117">Exclua cada limite de espaço em disco.</span><span class="sxs-lookup"><span data-stu-id="7e979-117">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="7e979-118">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="7e979-118">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="7e979-119">2</span><span class="sxs-lookup"><span data-stu-id="7e979-119">2</span></span>|<span data-ttu-id="7e979-120">Exclua cada limite de espaço em disco ou o limite inativa.</span><span class="sxs-lookup"><span data-stu-id="7e979-120">Delete at disk space threshold or inactive threshold.</span></span>|





