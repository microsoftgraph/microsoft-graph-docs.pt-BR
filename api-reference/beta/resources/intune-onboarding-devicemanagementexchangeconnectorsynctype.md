---
title: tipo de enumeração deviceManagementExchangeConnectorSyncType
description: O tipo de sincronização do Exchange Connector solicitada.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a4cb695d129f77409bfc83d902c10f2af511a86b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49307434"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="eae76-103">tipo de enumeração deviceManagementExchangeConnectorSyncType</span><span class="sxs-lookup"><span data-stu-id="eae76-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

<span data-ttu-id="eae76-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eae76-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eae76-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eae76-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eae76-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eae76-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eae76-107">O tipo de sincronização do Exchange Connector solicitada.</span><span class="sxs-lookup"><span data-stu-id="eae76-107">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="eae76-108">Membros</span><span class="sxs-lookup"><span data-stu-id="eae76-108">Members</span></span>
|<span data-ttu-id="eae76-109">Membro</span><span class="sxs-lookup"><span data-stu-id="eae76-109">Member</span></span>|<span data-ttu-id="eae76-110">Valor</span><span class="sxs-lookup"><span data-stu-id="eae76-110">Value</span></span>|<span data-ttu-id="eae76-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="eae76-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eae76-112">fullSync</span><span class="sxs-lookup"><span data-stu-id="eae76-112">fullSync</span></span>|<span data-ttu-id="eae76-113">,0</span><span class="sxs-lookup"><span data-stu-id="eae76-113">0</span></span>|<span data-ttu-id="eae76-114">Descubra todos os dispositivos no Exchange.</span><span class="sxs-lookup"><span data-stu-id="eae76-114">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="eae76-115">deltaSync</span><span class="sxs-lookup"><span data-stu-id="eae76-115">deltaSync</span></span>|<span data-ttu-id="eae76-116">1</span><span class="sxs-lookup"><span data-stu-id="eae76-116">1</span></span>|<span data-ttu-id="eae76-117">Descubra apenas o dispositivo no Exchange que foi atualizado durante a janela de sincronização Delta.</span><span class="sxs-lookup"><span data-stu-id="eae76-117">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|




