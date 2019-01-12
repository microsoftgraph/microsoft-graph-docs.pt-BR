---
title: tipo de enum sharedPCAccountDeletionPolicyType
description: Valores possíveis para quando as contas são excluídas em um PC compartilhado.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 081069f9462c426f24a1e3cf276730b1db40b191
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951947"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="5f462-103">tipo de enum sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="5f462-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="5f462-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5f462-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f462-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5f462-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5f462-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5f462-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5f462-107">Valores possíveis para quando as contas são excluídas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="5f462-107">Possible values for when accounts are deleted on a shared PC.</span></span>
## <a name="members"></a><span data-ttu-id="5f462-108">Membros</span><span class="sxs-lookup"><span data-stu-id="5f462-108">Members</span></span>
|<span data-ttu-id="5f462-109">Membro</span><span class="sxs-lookup"><span data-stu-id="5f462-109">Member</span></span>|<span data-ttu-id="5f462-110">Valor</span><span class="sxs-lookup"><span data-stu-id="5f462-110">Value</span></span>|<span data-ttu-id="5f462-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f462-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f462-112">imediata</span><span class="sxs-lookup"><span data-stu-id="5f462-112">immediate</span></span>|<span data-ttu-id="5f462-113">0</span><span class="sxs-lookup"><span data-stu-id="5f462-113">0</span></span>|<span data-ttu-id="5f462-114">Exclua imediatamente.</span><span class="sxs-lookup"><span data-stu-id="5f462-114">Delete immediately.</span></span>|
|<span data-ttu-id="5f462-115">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="5f462-115">diskSpaceThreshold</span></span>|<span data-ttu-id="5f462-116">1</span><span class="sxs-lookup"><span data-stu-id="5f462-116">1</span></span>|<span data-ttu-id="5f462-117">Exclua cada limite de espaço em disco.</span><span class="sxs-lookup"><span data-stu-id="5f462-117">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="5f462-118">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="5f462-118">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="5f462-119">2</span><span class="sxs-lookup"><span data-stu-id="5f462-119">2</span></span>|<span data-ttu-id="5f462-120">Exclua cada limite de espaço em disco ou o limite inativa.</span><span class="sxs-lookup"><span data-stu-id="5f462-120">Delete at disk space threshold or inactive threshold.</span></span>|





