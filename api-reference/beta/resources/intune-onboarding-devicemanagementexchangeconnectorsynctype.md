---
title: tipo de enumeração deviceManagementExchangeConnectorSyncType
description: O tipo de sincronização do Exchange Connector solicitada.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 04cd9e55b03e21bd4e99c56144ea05cabd1ecd7b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993001"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="f5380-103">tipo de enumeração deviceManagementExchangeConnectorSyncType</span><span class="sxs-lookup"><span data-stu-id="f5380-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="f5380-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f5380-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5380-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f5380-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5380-106">O tipo de sincronização do Exchange Connector solicitada.</span><span class="sxs-lookup"><span data-stu-id="f5380-106">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="f5380-107">Membros</span><span class="sxs-lookup"><span data-stu-id="f5380-107">Members</span></span>
|<span data-ttu-id="f5380-108">Membro</span><span class="sxs-lookup"><span data-stu-id="f5380-108">Member</span></span>|<span data-ttu-id="f5380-109">Valor</span><span class="sxs-lookup"><span data-stu-id="f5380-109">Value</span></span>|<span data-ttu-id="f5380-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5380-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5380-111">fullSync</span><span class="sxs-lookup"><span data-stu-id="f5380-111">fullSync</span></span>|<span data-ttu-id="f5380-112">,0</span><span class="sxs-lookup"><span data-stu-id="f5380-112">0</span></span>|<span data-ttu-id="f5380-113">Descubra todos os dispositivos no Exchange.</span><span class="sxs-lookup"><span data-stu-id="f5380-113">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="f5380-114">deltaSync</span><span class="sxs-lookup"><span data-stu-id="f5380-114">deltaSync</span></span>|<span data-ttu-id="f5380-115">1</span><span class="sxs-lookup"><span data-stu-id="f5380-115">1</span></span>|<span data-ttu-id="f5380-116">Descubra apenas o dispositivo no Exchange que foi atualizado durante a janela de sincronização Delta.</span><span class="sxs-lookup"><span data-stu-id="f5380-116">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|





