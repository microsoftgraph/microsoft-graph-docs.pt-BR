---
title: tipo de enumeração configurationManagerActionDeliveryStatus
description: Estado de entrega da ação de dispositivo do Gerenciador de configurações
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 09c7b1be3a5fdfc33a064d2a9208daa68ba4263e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733983"
---
# <a name="configurationmanageractiondeliverystatus-enum-type"></a><span data-ttu-id="a94b4-103">tipo de enumeração configurationManagerActionDeliveryStatus</span><span class="sxs-lookup"><span data-stu-id="a94b4-103">configurationManagerActionDeliveryStatus enum type</span></span>

<span data-ttu-id="a94b4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a94b4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a94b4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a94b4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a94b4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a94b4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a94b4-107">Estado de entrega da ação de dispositivo do Gerenciador de configurações</span><span class="sxs-lookup"><span data-stu-id="a94b4-107">Delivery state of Configuration Manager device action</span></span>

## <a name="members"></a><span data-ttu-id="a94b4-108">Membros</span><span class="sxs-lookup"><span data-stu-id="a94b4-108">Members</span></span>
|<span data-ttu-id="a94b4-109">Membro</span><span class="sxs-lookup"><span data-stu-id="a94b4-109">Member</span></span>|<span data-ttu-id="a94b4-110">Valor</span><span class="sxs-lookup"><span data-stu-id="a94b4-110">Value</span></span>|<span data-ttu-id="a94b4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a94b4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a94b4-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="a94b4-112">unknown</span></span>|<span data-ttu-id="a94b4-113">,0</span><span class="sxs-lookup"><span data-stu-id="a94b4-113">0</span></span>|<span data-ttu-id="a94b4-114">Pendente para entregar a ação a ConfigurationManager</span><span class="sxs-lookup"><span data-stu-id="a94b4-114">Pending to deliver the action to ConfigurationManager</span></span>|
|<span data-ttu-id="a94b4-115">pendingDelivery</span><span class="sxs-lookup"><span data-stu-id="a94b4-115">pendingDelivery</span></span>|<span data-ttu-id="a94b4-116">1</span><span class="sxs-lookup"><span data-stu-id="a94b4-116">1</span></span>|<span data-ttu-id="a94b4-117">Pendente para entregar a ação a ConfigurationManager</span><span class="sxs-lookup"><span data-stu-id="a94b4-117">Pending to deliver the action to ConfigurationManager</span></span>|
|<span data-ttu-id="a94b4-118">deliveredToConnectorService</span><span class="sxs-lookup"><span data-stu-id="a94b4-118">deliveredToConnectorService</span></span>|<span data-ttu-id="a94b4-119">duas</span><span class="sxs-lookup"><span data-stu-id="a94b4-119">2</span></span>|<span data-ttu-id="a94b4-120">A ação é enviada para o serviço do conector ConfigurationManager (nuvem)</span><span class="sxs-lookup"><span data-stu-id="a94b4-120">Action is sent to ConfigurationManager Connector service (cloud)</span></span>|
|<span data-ttu-id="a94b4-121">failedToDeliverToConnectorService</span><span class="sxs-lookup"><span data-stu-id="a94b4-121">failedToDeliverToConnectorService</span></span>|<span data-ttu-id="a94b4-122">3D</span><span class="sxs-lookup"><span data-stu-id="a94b4-122">3</span></span>|<span data-ttu-id="a94b4-123">Falha ao enviar a ação para o serviço do conector ConfigurationManager (nuvem)</span><span class="sxs-lookup"><span data-stu-id="a94b4-123">Failed to send the action to ConfigurationManager Connector service (cloud)</span></span>|
|<span data-ttu-id="a94b4-124">deliveredToOnPremisesServer</span><span class="sxs-lookup"><span data-stu-id="a94b4-124">deliveredToOnPremisesServer</span></span>|<span data-ttu-id="a94b4-125">4 </span><span class="sxs-lookup"><span data-stu-id="a94b4-125">4</span></span>|<span data-ttu-id="a94b4-126">A ação é entregue no servidor local do ConfigurationManager</span><span class="sxs-lookup"><span data-stu-id="a94b4-126">Action is delivered to ConfigurationManager on-prem server</span></span>|





