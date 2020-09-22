---
title: tipo de enumeração deviceManagementExchangeConnectorSyncType
description: O tipo de sincronização do Exchange Connector solicitada.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 12223e48d60fffbfa0ad3b222b490c3e59295094
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029614"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="cb671-103">tipo de enumeração deviceManagementExchangeConnectorSyncType</span><span class="sxs-lookup"><span data-stu-id="cb671-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

<span data-ttu-id="cb671-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb671-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cb671-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cb671-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb671-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cb671-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb671-107">O tipo de sincronização do Exchange Connector solicitada.</span><span class="sxs-lookup"><span data-stu-id="cb671-107">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="cb671-108">Membros</span><span class="sxs-lookup"><span data-stu-id="cb671-108">Members</span></span>
|<span data-ttu-id="cb671-109">Membro</span><span class="sxs-lookup"><span data-stu-id="cb671-109">Member</span></span>|<span data-ttu-id="cb671-110">Valor</span><span class="sxs-lookup"><span data-stu-id="cb671-110">Value</span></span>|<span data-ttu-id="cb671-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb671-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb671-112">fullSync</span><span class="sxs-lookup"><span data-stu-id="cb671-112">fullSync</span></span>|<span data-ttu-id="cb671-113">,0</span><span class="sxs-lookup"><span data-stu-id="cb671-113">0</span></span>|<span data-ttu-id="cb671-114">Descubra todos os dispositivos no Exchange.</span><span class="sxs-lookup"><span data-stu-id="cb671-114">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="cb671-115">deltaSync</span><span class="sxs-lookup"><span data-stu-id="cb671-115">deltaSync</span></span>|<span data-ttu-id="cb671-116">1 </span><span class="sxs-lookup"><span data-stu-id="cb671-116">1</span></span>|<span data-ttu-id="cb671-117">Descubra apenas o dispositivo no Exchange que foi atualizado durante a janela de sincronização Delta.</span><span class="sxs-lookup"><span data-stu-id="cb671-117">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|






