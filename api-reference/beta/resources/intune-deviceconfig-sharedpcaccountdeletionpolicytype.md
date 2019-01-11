---
title: tipo de enum sharedPCAccountDeletionPolicyType
description: Valores possíveis para quando as contas são excluídas em um PC compartilhado.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d7f51f76e6164c973b213eb53526d5961bb2b627
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861030"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="e6944-103">tipo de enum sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="e6944-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="e6944-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e6944-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e6944-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e6944-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e6944-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e6944-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e6944-107">Valores possíveis para quando as contas são excluídas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="e6944-107">Possible values for when accounts are deleted on a shared PC.</span></span>
## <a name="members"></a><span data-ttu-id="e6944-108">Membros</span><span class="sxs-lookup"><span data-stu-id="e6944-108">Members</span></span>
|<span data-ttu-id="e6944-109">Membro</span><span class="sxs-lookup"><span data-stu-id="e6944-109">Member</span></span>|<span data-ttu-id="e6944-110">Valor</span><span class="sxs-lookup"><span data-stu-id="e6944-110">Value</span></span>|<span data-ttu-id="e6944-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6944-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6944-112">imediata</span><span class="sxs-lookup"><span data-stu-id="e6944-112">immediate</span></span>|<span data-ttu-id="e6944-113">0</span><span class="sxs-lookup"><span data-stu-id="e6944-113">0</span></span>|<span data-ttu-id="e6944-114">Exclua imediatamente.</span><span class="sxs-lookup"><span data-stu-id="e6944-114">Delete immediately.</span></span>|
|<span data-ttu-id="e6944-115">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="e6944-115">diskSpaceThreshold</span></span>|<span data-ttu-id="e6944-116">1</span><span class="sxs-lookup"><span data-stu-id="e6944-116">1</span></span>|<span data-ttu-id="e6944-117">Exclua cada limite de espaço em disco.</span><span class="sxs-lookup"><span data-stu-id="e6944-117">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="e6944-118">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="e6944-118">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="e6944-119">2</span><span class="sxs-lookup"><span data-stu-id="e6944-119">2</span></span>|<span data-ttu-id="e6944-120">Exclua cada limite de espaço em disco ou o limite inativa.</span><span class="sxs-lookup"><span data-stu-id="e6944-120">Delete at disk space threshold or inactive threshold.</span></span>|





