---
title: tipo de enumeração deviceManagementExchangeConnectorSyncType
description: O tipo de sincronização do Exchange Connector solicitada.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cfdd1da2ecec6fb7848787386991ee09741d0b67
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565923"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="77f3b-103">tipo de enumeração deviceManagementExchangeConnectorSyncType</span><span class="sxs-lookup"><span data-stu-id="77f3b-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="77f3b-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="77f3b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77f3b-105">O tipo de sincronização do Exchange Connector solicitada.</span><span class="sxs-lookup"><span data-stu-id="77f3b-105">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="77f3b-106">Membros</span><span class="sxs-lookup"><span data-stu-id="77f3b-106">Members</span></span>
|<span data-ttu-id="77f3b-107">Membro</span><span class="sxs-lookup"><span data-stu-id="77f3b-107">Member</span></span>|<span data-ttu-id="77f3b-108">Valor</span><span class="sxs-lookup"><span data-stu-id="77f3b-108">Value</span></span>|<span data-ttu-id="77f3b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="77f3b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77f3b-110">fullSync</span><span class="sxs-lookup"><span data-stu-id="77f3b-110">fullSync</span></span>|<span data-ttu-id="77f3b-111">,0</span><span class="sxs-lookup"><span data-stu-id="77f3b-111">0</span></span>|<span data-ttu-id="77f3b-112">Descubra todos os dispositivos no Exchange.</span><span class="sxs-lookup"><span data-stu-id="77f3b-112">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="77f3b-113">deltaSync</span><span class="sxs-lookup"><span data-stu-id="77f3b-113">deltaSync</span></span>|<span data-ttu-id="77f3b-114">1 </span><span class="sxs-lookup"><span data-stu-id="77f3b-114">1</span></span>|<span data-ttu-id="77f3b-115">Descubra apenas o dispositivo no Exchange que foi atualizado durante a janela de sincronização Delta.</span><span class="sxs-lookup"><span data-stu-id="77f3b-115">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|



