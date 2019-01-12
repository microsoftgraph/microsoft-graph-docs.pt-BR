---
title: tipo de enum deviceManagementExchangeConnectorType
description: O tipo de conector do Exchange.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8e9e50a4475ca2d57b3f38567703046588d4fb3c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986429"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="77985-103">tipo de enum deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="77985-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="77985-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="77985-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="77985-105">O tipo de conector do Exchange.</span><span class="sxs-lookup"><span data-stu-id="77985-105">The type of Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="77985-106">Membros</span><span class="sxs-lookup"><span data-stu-id="77985-106">Members</span></span>
|<span data-ttu-id="77985-107">Membro</span><span class="sxs-lookup"><span data-stu-id="77985-107">Member</span></span>|<span data-ttu-id="77985-108">Valor</span><span class="sxs-lookup"><span data-stu-id="77985-108">Value</span></span>|<span data-ttu-id="77985-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="77985-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77985-110">onPremises</span><span class="sxs-lookup"><span data-stu-id="77985-110">onPremises</span></span>|<span data-ttu-id="77985-111">0</span><span class="sxs-lookup"><span data-stu-id="77985-111">0</span></span>|<span data-ttu-id="77985-112">Conecta-se ao ambiente do Exchange local.</span><span class="sxs-lookup"><span data-stu-id="77985-112">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="77985-113">hospedado</span><span class="sxs-lookup"><span data-stu-id="77985-113">hosted</span></span>|<span data-ttu-id="77985-114">1</span><span class="sxs-lookup"><span data-stu-id="77985-114">1</span></span>|<span data-ttu-id="77985-115">Conecta-se ao ambiente do Exchange de multilocatário O365</span><span class="sxs-lookup"><span data-stu-id="77985-115">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="77985-116">serviceToService</span><span class="sxs-lookup"><span data-stu-id="77985-116">serviceToService</span></span>|<span data-ttu-id="77985-117">2</span><span class="sxs-lookup"><span data-stu-id="77985-117">2</span></span>|<span data-ttu-id="77985-118">Intune Service se conectará diretamente ao ambiente do Exchange de multilocatário O365</span><span class="sxs-lookup"><span data-stu-id="77985-118">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="77985-119">dedicada</span><span class="sxs-lookup"><span data-stu-id="77985-119">dedicated</span></span>|<span data-ttu-id="77985-120">3</span><span class="sxs-lookup"><span data-stu-id="77985-120">3</span></span>|<span data-ttu-id="77985-121">Conecta-se ao ambiente do Exchange dedicada do O365.</span><span class="sxs-lookup"><span data-stu-id="77985-121">Connects to O365 Dedicated Exchange environment.</span></span>|



