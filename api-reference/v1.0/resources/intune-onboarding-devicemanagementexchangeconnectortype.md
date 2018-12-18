---
title: tipo de enum deviceManagementExchangeConnectorType
description: O tipo de conector do Exchange.
author: tfitzmac
ms.openlocfilehash: 333a5a7c6f73fead263edbdf3edafeefc3514ed1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306731"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="ffe54-103">tipo de enum deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="ffe54-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="ffe54-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ffe54-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ffe54-105">O tipo de conector do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ffe54-105">The type of Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="ffe54-106">Membros</span><span class="sxs-lookup"><span data-stu-id="ffe54-106">Members</span></span>
|<span data-ttu-id="ffe54-107">Membro</span><span class="sxs-lookup"><span data-stu-id="ffe54-107">Member</span></span>|<span data-ttu-id="ffe54-108">Valor</span><span class="sxs-lookup"><span data-stu-id="ffe54-108">Value</span></span>|<span data-ttu-id="ffe54-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ffe54-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffe54-110">onPremises</span><span class="sxs-lookup"><span data-stu-id="ffe54-110">onPremises</span></span>|<span data-ttu-id="ffe54-111">0</span><span class="sxs-lookup"><span data-stu-id="ffe54-111">0</span></span>|<span data-ttu-id="ffe54-112">Conecta-se ao ambiente do Exchange local.</span><span class="sxs-lookup"><span data-stu-id="ffe54-112">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="ffe54-113">hospedado</span><span class="sxs-lookup"><span data-stu-id="ffe54-113">hosted</span></span>|<span data-ttu-id="ffe54-114">1</span><span class="sxs-lookup"><span data-stu-id="ffe54-114">1</span></span>|<span data-ttu-id="ffe54-115">Conecta-se ao ambiente do Exchange de multilocatário O365</span><span class="sxs-lookup"><span data-stu-id="ffe54-115">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="ffe54-116">serviceToService</span><span class="sxs-lookup"><span data-stu-id="ffe54-116">serviceToService</span></span>|<span data-ttu-id="ffe54-117">2</span><span class="sxs-lookup"><span data-stu-id="ffe54-117">2</span></span>|<span data-ttu-id="ffe54-118">Intune Service se conectará diretamente ao ambiente do Exchange de multilocatário O365</span><span class="sxs-lookup"><span data-stu-id="ffe54-118">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="ffe54-119">dedicada</span><span class="sxs-lookup"><span data-stu-id="ffe54-119">dedicated</span></span>|<span data-ttu-id="ffe54-120">3</span><span class="sxs-lookup"><span data-stu-id="ffe54-120">3</span></span>|<span data-ttu-id="ffe54-121">Conecta-se ao ambiente do Exchange dedicada do O365.</span><span class="sxs-lookup"><span data-stu-id="ffe54-121">Connects to O365 Dedicated Exchange environment.</span></span>|



