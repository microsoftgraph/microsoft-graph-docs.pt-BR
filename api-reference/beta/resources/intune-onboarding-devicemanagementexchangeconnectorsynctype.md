---
title: tipo de enumeração deviceManagementExchangeConnectorSyncType
description: O tipo de sincronização do Exchange Connector solicitada.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f68277b2eeb7aea123ee843a0b602d11123cbd04
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369448"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="e4c39-103">tipo de enumeração deviceManagementExchangeConnectorSyncType</span><span class="sxs-lookup"><span data-stu-id="e4c39-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="e4c39-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e4c39-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4c39-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e4c39-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4c39-106">O tipo de sincronização do Exchange Connector solicitada.</span><span class="sxs-lookup"><span data-stu-id="e4c39-106">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="e4c39-107">Membros</span><span class="sxs-lookup"><span data-stu-id="e4c39-107">Members</span></span>
|<span data-ttu-id="e4c39-108">Membro</span><span class="sxs-lookup"><span data-stu-id="e4c39-108">Member</span></span>|<span data-ttu-id="e4c39-109">Valor</span><span class="sxs-lookup"><span data-stu-id="e4c39-109">Value</span></span>|<span data-ttu-id="e4c39-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4c39-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4c39-111">fullSync</span><span class="sxs-lookup"><span data-stu-id="e4c39-111">fullSync</span></span>|<span data-ttu-id="e4c39-112">,0</span><span class="sxs-lookup"><span data-stu-id="e4c39-112">0</span></span>|<span data-ttu-id="e4c39-113">Descubra todos os dispositivos no Exchange.</span><span class="sxs-lookup"><span data-stu-id="e4c39-113">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="e4c39-114">deltaSync</span><span class="sxs-lookup"><span data-stu-id="e4c39-114">deltaSync</span></span>|<span data-ttu-id="e4c39-115">1</span><span class="sxs-lookup"><span data-stu-id="e4c39-115">1</span></span>|<span data-ttu-id="e4c39-116">Descubra apenas o dispositivo no Exchange que foi atualizado durante a janela de sincronização Delta.</span><span class="sxs-lookup"><span data-stu-id="e4c39-116">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|



