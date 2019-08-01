---
title: tipo de enumeração deviceManagementExchangeConnectorSyncType
description: O tipo de sincronização do Exchange Connector solicitada.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0066b6b4fce924df8c5101228db8868da7e1b743
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037440"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="962bd-103">tipo de enumeração deviceManagementExchangeConnectorSyncType</span><span class="sxs-lookup"><span data-stu-id="962bd-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="962bd-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="962bd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="962bd-105">O tipo de sincronização do Exchange Connector solicitada.</span><span class="sxs-lookup"><span data-stu-id="962bd-105">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="962bd-106">Membros</span><span class="sxs-lookup"><span data-stu-id="962bd-106">Members</span></span>
|<span data-ttu-id="962bd-107">Membro</span><span class="sxs-lookup"><span data-stu-id="962bd-107">Member</span></span>|<span data-ttu-id="962bd-108">Valor</span><span class="sxs-lookup"><span data-stu-id="962bd-108">Value</span></span>|<span data-ttu-id="962bd-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="962bd-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="962bd-110">fullSync</span><span class="sxs-lookup"><span data-stu-id="962bd-110">fullSync</span></span>|<span data-ttu-id="962bd-111">,0</span><span class="sxs-lookup"><span data-stu-id="962bd-111">0</span></span>|<span data-ttu-id="962bd-112">Descubra todos os dispositivos no Exchange.</span><span class="sxs-lookup"><span data-stu-id="962bd-112">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="962bd-113">deltaSync</span><span class="sxs-lookup"><span data-stu-id="962bd-113">deltaSync</span></span>|<span data-ttu-id="962bd-114">1</span><span class="sxs-lookup"><span data-stu-id="962bd-114">1</span></span>|<span data-ttu-id="962bd-115">Descubra apenas o dispositivo no Exchange que foi atualizado durante a janela de sincronização Delta.</span><span class="sxs-lookup"><span data-stu-id="962bd-115">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|



