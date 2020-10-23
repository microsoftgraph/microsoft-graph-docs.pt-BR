---
title: tipo de enumeração deviceManagementExchangeConnectorSyncType
description: O tipo de sincronização do Exchange Connector solicitada.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 6598b2bc7a6ee4c75c201ec86718f933696f7f1c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736097"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="0e6d2-103">tipo de enumeração deviceManagementExchangeConnectorSyncType</span><span class="sxs-lookup"><span data-stu-id="0e6d2-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

<span data-ttu-id="0e6d2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e6d2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0e6d2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0e6d2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e6d2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0e6d2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e6d2-107">O tipo de sincronização do Exchange Connector solicitada.</span><span class="sxs-lookup"><span data-stu-id="0e6d2-107">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="0e6d2-108">Membros</span><span class="sxs-lookup"><span data-stu-id="0e6d2-108">Members</span></span>
|<span data-ttu-id="0e6d2-109">Membro</span><span class="sxs-lookup"><span data-stu-id="0e6d2-109">Member</span></span>|<span data-ttu-id="0e6d2-110">Valor</span><span class="sxs-lookup"><span data-stu-id="0e6d2-110">Value</span></span>|<span data-ttu-id="0e6d2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e6d2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e6d2-112">fullSync</span><span class="sxs-lookup"><span data-stu-id="0e6d2-112">fullSync</span></span>|<span data-ttu-id="0e6d2-113">,0</span><span class="sxs-lookup"><span data-stu-id="0e6d2-113">0</span></span>|<span data-ttu-id="0e6d2-114">Descubra todos os dispositivos no Exchange.</span><span class="sxs-lookup"><span data-stu-id="0e6d2-114">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="0e6d2-115">deltaSync</span><span class="sxs-lookup"><span data-stu-id="0e6d2-115">deltaSync</span></span>|<span data-ttu-id="0e6d2-116">1</span><span class="sxs-lookup"><span data-stu-id="0e6d2-116">1</span></span>|<span data-ttu-id="0e6d2-117">Descubra apenas o dispositivo no Exchange que foi atualizado durante a janela de sincronização Delta.</span><span class="sxs-lookup"><span data-stu-id="0e6d2-117">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|





