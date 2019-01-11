---
title: tipo de enum deviceManagementExchangeConnectorType
description: O tipo de conector do Exchange.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 07449df53aa65036ae55e63c514c1687fbbab86a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888512"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="86246-103">tipo de enum deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="86246-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="86246-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="86246-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="86246-105">O tipo de conector do Exchange.</span><span class="sxs-lookup"><span data-stu-id="86246-105">The type of Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="86246-106">Membros</span><span class="sxs-lookup"><span data-stu-id="86246-106">Members</span></span>
|<span data-ttu-id="86246-107">Membro</span><span class="sxs-lookup"><span data-stu-id="86246-107">Member</span></span>|<span data-ttu-id="86246-108">Valor</span><span class="sxs-lookup"><span data-stu-id="86246-108">Value</span></span>|<span data-ttu-id="86246-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="86246-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86246-110">onPremises</span><span class="sxs-lookup"><span data-stu-id="86246-110">onPremises</span></span>|<span data-ttu-id="86246-111">0</span><span class="sxs-lookup"><span data-stu-id="86246-111">0</span></span>|<span data-ttu-id="86246-112">Conecta-se ao ambiente do Exchange local.</span><span class="sxs-lookup"><span data-stu-id="86246-112">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="86246-113">hospedado</span><span class="sxs-lookup"><span data-stu-id="86246-113">hosted</span></span>|<span data-ttu-id="86246-114">1</span><span class="sxs-lookup"><span data-stu-id="86246-114">1</span></span>|<span data-ttu-id="86246-115">Conecta-se ao ambiente do Exchange de multilocatário O365</span><span class="sxs-lookup"><span data-stu-id="86246-115">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="86246-116">serviceToService</span><span class="sxs-lookup"><span data-stu-id="86246-116">serviceToService</span></span>|<span data-ttu-id="86246-117">2</span><span class="sxs-lookup"><span data-stu-id="86246-117">2</span></span>|<span data-ttu-id="86246-118">Intune Service se conectará diretamente ao ambiente do Exchange de multilocatário O365</span><span class="sxs-lookup"><span data-stu-id="86246-118">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="86246-119">dedicada</span><span class="sxs-lookup"><span data-stu-id="86246-119">dedicated</span></span>|<span data-ttu-id="86246-120">3</span><span class="sxs-lookup"><span data-stu-id="86246-120">3</span></span>|<span data-ttu-id="86246-121">Conecta-se ao ambiente do Exchange dedicada do O365.</span><span class="sxs-lookup"><span data-stu-id="86246-121">Connects to O365 Dedicated Exchange environment.</span></span>|



