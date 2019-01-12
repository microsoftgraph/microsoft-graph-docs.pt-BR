---
title: tipo de enum deviceManagementExchangeConnectorType
description: O tipo de conector do Exchange.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c05410c3b3b7c889840d0b47aca05f6457564eb4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934948"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="99254-103">tipo de enum deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="99254-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="99254-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="99254-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99254-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="99254-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="99254-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="99254-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="99254-107">O tipo de conector do Exchange.</span><span class="sxs-lookup"><span data-stu-id="99254-107">The type of Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="99254-108">Membros</span><span class="sxs-lookup"><span data-stu-id="99254-108">Members</span></span>
|<span data-ttu-id="99254-109">Membro</span><span class="sxs-lookup"><span data-stu-id="99254-109">Member</span></span>|<span data-ttu-id="99254-110">Valor</span><span class="sxs-lookup"><span data-stu-id="99254-110">Value</span></span>|<span data-ttu-id="99254-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="99254-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99254-112">onPremises</span><span class="sxs-lookup"><span data-stu-id="99254-112">onPremises</span></span>|<span data-ttu-id="99254-113">0</span><span class="sxs-lookup"><span data-stu-id="99254-113">0</span></span>|<span data-ttu-id="99254-114">Conecta-se ao ambiente do Exchange local.</span><span class="sxs-lookup"><span data-stu-id="99254-114">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="99254-115">hospedado</span><span class="sxs-lookup"><span data-stu-id="99254-115">hosted</span></span>|<span data-ttu-id="99254-116">1</span><span class="sxs-lookup"><span data-stu-id="99254-116">1</span></span>|<span data-ttu-id="99254-117">Conecta-se ao ambiente do Exchange de multilocatário O365</span><span class="sxs-lookup"><span data-stu-id="99254-117">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="99254-118">serviceToService</span><span class="sxs-lookup"><span data-stu-id="99254-118">serviceToService</span></span>|<span data-ttu-id="99254-119">2</span><span class="sxs-lookup"><span data-stu-id="99254-119">2</span></span>|<span data-ttu-id="99254-120">Intune Service se conectará diretamente ao ambiente do Exchange de multilocatário O365</span><span class="sxs-lookup"><span data-stu-id="99254-120">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="99254-121">dedicada</span><span class="sxs-lookup"><span data-stu-id="99254-121">dedicated</span></span>|<span data-ttu-id="99254-122">3</span><span class="sxs-lookup"><span data-stu-id="99254-122">3</span></span>|<span data-ttu-id="99254-123">Conecta-se ao ambiente do Exchange dedicada do O365.</span><span class="sxs-lookup"><span data-stu-id="99254-123">Connects to O365 Dedicated Exchange environment.</span></span>|





