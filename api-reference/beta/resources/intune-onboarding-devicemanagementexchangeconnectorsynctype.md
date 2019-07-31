---
title: tipo de enumeração deviceManagementExchangeConnectorSyncType
description: O tipo de sincronização do Exchange Connector solicitada.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 86cdc6277232985d4c3e247c5c14801a5d3aef54
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010760"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="e5ef4-103">tipo de enumeração deviceManagementExchangeConnectorSyncType</span><span class="sxs-lookup"><span data-stu-id="e5ef4-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="e5ef4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e5ef4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5ef4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e5ef4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5ef4-106">O tipo de sincronização do Exchange Connector solicitada.</span><span class="sxs-lookup"><span data-stu-id="e5ef4-106">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="e5ef4-107">Membros</span><span class="sxs-lookup"><span data-stu-id="e5ef4-107">Members</span></span>
|<span data-ttu-id="e5ef4-108">Membro</span><span class="sxs-lookup"><span data-stu-id="e5ef4-108">Member</span></span>|<span data-ttu-id="e5ef4-109">Valor</span><span class="sxs-lookup"><span data-stu-id="e5ef4-109">Value</span></span>|<span data-ttu-id="e5ef4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5ef4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5ef4-111">fullSync</span><span class="sxs-lookup"><span data-stu-id="e5ef4-111">fullSync</span></span>|<span data-ttu-id="e5ef4-112">,0</span><span class="sxs-lookup"><span data-stu-id="e5ef4-112">0</span></span>|<span data-ttu-id="e5ef4-113">Descubra todos os dispositivos no Exchange.</span><span class="sxs-lookup"><span data-stu-id="e5ef4-113">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="e5ef4-114">deltaSync</span><span class="sxs-lookup"><span data-stu-id="e5ef4-114">deltaSync</span></span>|<span data-ttu-id="e5ef4-115">1</span><span class="sxs-lookup"><span data-stu-id="e5ef4-115">1</span></span>|<span data-ttu-id="e5ef4-116">Descubra apenas o dispositivo no Exchange que foi atualizado durante a janela de sincronização Delta.</span><span class="sxs-lookup"><span data-stu-id="e5ef4-116">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|





