---
title: tipo de enumeração configurationManagerActionDeliveryStatus
description: Estado de entrega da ação de dispositivo do Gerenciador de configurações
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 58dca2b1ecb5419a3f56889a55c0816f492af430
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785088"
---
# <a name="configurationmanageractiondeliverystatus-enum-type"></a><span data-ttu-id="58654-103">tipo de enumeração configurationManagerActionDeliveryStatus</span><span class="sxs-lookup"><span data-stu-id="58654-103">configurationManagerActionDeliveryStatus enum type</span></span>

> <span data-ttu-id="58654-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="58654-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58654-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="58654-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58654-106">Estado de entrega da ação de dispositivo do Gerenciador de configurações</span><span class="sxs-lookup"><span data-stu-id="58654-106">Delivery state of Configuration Manager device action</span></span>

## <a name="members"></a><span data-ttu-id="58654-107">Membros</span><span class="sxs-lookup"><span data-stu-id="58654-107">Members</span></span>
|<span data-ttu-id="58654-108">Membro</span><span class="sxs-lookup"><span data-stu-id="58654-108">Member</span></span>|<span data-ttu-id="58654-109">Valor</span><span class="sxs-lookup"><span data-stu-id="58654-109">Value</span></span>|<span data-ttu-id="58654-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="58654-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58654-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="58654-111">unknown</span></span>|<span data-ttu-id="58654-112">,0</span><span class="sxs-lookup"><span data-stu-id="58654-112">0</span></span>|<span data-ttu-id="58654-113">Pendente para entregar a ação a ConfigurationManager</span><span class="sxs-lookup"><span data-stu-id="58654-113">Pending to deliver the action to ConfigurationManager</span></span>|
|<span data-ttu-id="58654-114">pendingDelivery</span><span class="sxs-lookup"><span data-stu-id="58654-114">pendingDelivery</span></span>|<span data-ttu-id="58654-115">1</span><span class="sxs-lookup"><span data-stu-id="58654-115">1</span></span>|<span data-ttu-id="58654-116">Pendente para entregar a ação a ConfigurationManager</span><span class="sxs-lookup"><span data-stu-id="58654-116">Pending to deliver the action to ConfigurationManager</span></span>|
|<span data-ttu-id="58654-117">deliveredToConnectorService</span><span class="sxs-lookup"><span data-stu-id="58654-117">deliveredToConnectorService</span></span>|<span data-ttu-id="58654-118">duas</span><span class="sxs-lookup"><span data-stu-id="58654-118">2</span></span>|<span data-ttu-id="58654-119">A ação é enviada para o serviço do conector ConfigurationManager (nuvem)</span><span class="sxs-lookup"><span data-stu-id="58654-119">Action is sent to ConfigurationManager Connector service (cloud)</span></span>|
|<span data-ttu-id="58654-120">failedToDeliverToConnectorService</span><span class="sxs-lookup"><span data-stu-id="58654-120">failedToDeliverToConnectorService</span></span>|<span data-ttu-id="58654-121">3D</span><span class="sxs-lookup"><span data-stu-id="58654-121">3</span></span>|<span data-ttu-id="58654-122">Falha ao enviar a ação para o serviço do conector ConfigurationManager (nuvem)</span><span class="sxs-lookup"><span data-stu-id="58654-122">Failed to send the action to ConfigurationManager Connector service (cloud)</span></span>|
|<span data-ttu-id="58654-123">deliveredToOnPremisesServer</span><span class="sxs-lookup"><span data-stu-id="58654-123">deliveredToOnPremisesServer</span></span>|<span data-ttu-id="58654-124">4 </span><span class="sxs-lookup"><span data-stu-id="58654-124">4</span></span>|<span data-ttu-id="58654-125">A ação é entregue no servidor local do ConfigurationManager</span><span class="sxs-lookup"><span data-stu-id="58654-125">Action is delivered to ConfigurationManager on-prem server</span></span>|



