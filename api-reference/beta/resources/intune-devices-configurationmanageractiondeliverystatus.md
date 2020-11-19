---
title: tipo de enumeração configurationManagerActionDeliveryStatus
description: Estado de entrega da ação de dispositivo do Gerenciador de configurações
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: bbe36a6f7e346467d35bf997817241d7f30ef6df
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214621"
---
# <a name="configurationmanageractiondeliverystatus-enum-type"></a><span data-ttu-id="04a07-103">tipo de enumeração configurationManagerActionDeliveryStatus</span><span class="sxs-lookup"><span data-stu-id="04a07-103">configurationManagerActionDeliveryStatus enum type</span></span>

<span data-ttu-id="04a07-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04a07-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="04a07-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="04a07-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04a07-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="04a07-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04a07-107">Estado de entrega da ação de dispositivo do Gerenciador de configurações</span><span class="sxs-lookup"><span data-stu-id="04a07-107">Delivery state of Configuration Manager device action</span></span>

## <a name="members"></a><span data-ttu-id="04a07-108">Membros</span><span class="sxs-lookup"><span data-stu-id="04a07-108">Members</span></span>
|<span data-ttu-id="04a07-109">Membro</span><span class="sxs-lookup"><span data-stu-id="04a07-109">Member</span></span>|<span data-ttu-id="04a07-110">Valor</span><span class="sxs-lookup"><span data-stu-id="04a07-110">Value</span></span>|<span data-ttu-id="04a07-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="04a07-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04a07-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="04a07-112">unknown</span></span>|<span data-ttu-id="04a07-113">,0</span><span class="sxs-lookup"><span data-stu-id="04a07-113">0</span></span>|<span data-ttu-id="04a07-114">Pendente para entregar a ação a ConfigurationManager</span><span class="sxs-lookup"><span data-stu-id="04a07-114">Pending to deliver the action to ConfigurationManager</span></span>|
|<span data-ttu-id="04a07-115">pendingDelivery</span><span class="sxs-lookup"><span data-stu-id="04a07-115">pendingDelivery</span></span>|<span data-ttu-id="04a07-116">1</span><span class="sxs-lookup"><span data-stu-id="04a07-116">1</span></span>|<span data-ttu-id="04a07-117">Pendente para entregar a ação a ConfigurationManager</span><span class="sxs-lookup"><span data-stu-id="04a07-117">Pending to deliver the action to ConfigurationManager</span></span>|
|<span data-ttu-id="04a07-118">deliveredToConnectorService</span><span class="sxs-lookup"><span data-stu-id="04a07-118">deliveredToConnectorService</span></span>|<span data-ttu-id="04a07-119">duas</span><span class="sxs-lookup"><span data-stu-id="04a07-119">2</span></span>|<span data-ttu-id="04a07-120">A ação é enviada para o serviço do conector ConfigurationManager (nuvem)</span><span class="sxs-lookup"><span data-stu-id="04a07-120">Action is sent to ConfigurationManager Connector service (cloud)</span></span>|
|<span data-ttu-id="04a07-121">failedToDeliverToConnectorService</span><span class="sxs-lookup"><span data-stu-id="04a07-121">failedToDeliverToConnectorService</span></span>|<span data-ttu-id="04a07-122">3D</span><span class="sxs-lookup"><span data-stu-id="04a07-122">3</span></span>|<span data-ttu-id="04a07-123">Falha ao enviar a ação para o serviço do conector ConfigurationManager (nuvem)</span><span class="sxs-lookup"><span data-stu-id="04a07-123">Failed to send the action to ConfigurationManager Connector service (cloud)</span></span>|
|<span data-ttu-id="04a07-124">deliveredToOnPremisesServer</span><span class="sxs-lookup"><span data-stu-id="04a07-124">deliveredToOnPremisesServer</span></span>|<span data-ttu-id="04a07-125">4 </span><span class="sxs-lookup"><span data-stu-id="04a07-125">4</span></span>|<span data-ttu-id="04a07-126">A ação é entregue no servidor local do ConfigurationManager</span><span class="sxs-lookup"><span data-stu-id="04a07-126">Action is delivered to ConfigurationManager on-prem server</span></span>|




