---
title: tipo de enum deviceManagementExchangeConnectorSyncType
description: O tipo de sincronização do Exchange Connector solicitada.
author: tfitzmac
ms.openlocfilehash: 1915de3305cb8e41609dd2101f246a8e003f60f4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312072"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="55dc9-103">tipo de enum deviceManagementExchangeConnectorSyncType</span><span class="sxs-lookup"><span data-stu-id="55dc9-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="55dc9-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="55dc9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="55dc9-105">O tipo de sincronização do Exchange Connector solicitada.</span><span class="sxs-lookup"><span data-stu-id="55dc9-105">The type of Exchange Connector sync requested.</span></span>
## <a name="members"></a><span data-ttu-id="55dc9-106">Membros</span><span class="sxs-lookup"><span data-stu-id="55dc9-106">Members</span></span>
|<span data-ttu-id="55dc9-107">Membro</span><span class="sxs-lookup"><span data-stu-id="55dc9-107">Member</span></span>|<span data-ttu-id="55dc9-108">Valor</span><span class="sxs-lookup"><span data-stu-id="55dc9-108">Value</span></span>|<span data-ttu-id="55dc9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="55dc9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55dc9-110">fullSync</span><span class="sxs-lookup"><span data-stu-id="55dc9-110">fullSync</span></span>|<span data-ttu-id="55dc9-111">0</span><span class="sxs-lookup"><span data-stu-id="55dc9-111">0</span></span>|<span data-ttu-id="55dc9-112">Descubra todo o dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="55dc9-112">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="55dc9-113">deltaSync</span><span class="sxs-lookup"><span data-stu-id="55dc9-113">deltaSync</span></span>|<span data-ttu-id="55dc9-114">1</span><span class="sxs-lookup"><span data-stu-id="55dc9-114">1</span></span>|<span data-ttu-id="55dc9-115">Descobrir somente o dispositivo no Exchange que atualizou durante a janela de sincronização delta.</span><span class="sxs-lookup"><span data-stu-id="55dc9-115">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|



