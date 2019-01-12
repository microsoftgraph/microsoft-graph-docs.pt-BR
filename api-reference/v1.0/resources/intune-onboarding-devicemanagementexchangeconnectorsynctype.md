---
title: tipo de enum deviceManagementExchangeConnectorSyncType
description: O tipo de sincronização do Exchange Connector solicitada.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5af14006bd6f3cc8733faecc8e0219cc02e7fcd9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983279"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="342c1-103">tipo de enum deviceManagementExchangeConnectorSyncType</span><span class="sxs-lookup"><span data-stu-id="342c1-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="342c1-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="342c1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="342c1-105">O tipo de sincronização do Exchange Connector solicitada.</span><span class="sxs-lookup"><span data-stu-id="342c1-105">The type of Exchange Connector sync requested.</span></span>
## <a name="members"></a><span data-ttu-id="342c1-106">Membros</span><span class="sxs-lookup"><span data-stu-id="342c1-106">Members</span></span>
|<span data-ttu-id="342c1-107">Membro</span><span class="sxs-lookup"><span data-stu-id="342c1-107">Member</span></span>|<span data-ttu-id="342c1-108">Valor</span><span class="sxs-lookup"><span data-stu-id="342c1-108">Value</span></span>|<span data-ttu-id="342c1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="342c1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="342c1-110">fullSync</span><span class="sxs-lookup"><span data-stu-id="342c1-110">fullSync</span></span>|<span data-ttu-id="342c1-111">0</span><span class="sxs-lookup"><span data-stu-id="342c1-111">0</span></span>|<span data-ttu-id="342c1-112">Descubra todo o dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="342c1-112">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="342c1-113">deltaSync</span><span class="sxs-lookup"><span data-stu-id="342c1-113">deltaSync</span></span>|<span data-ttu-id="342c1-114">1</span><span class="sxs-lookup"><span data-stu-id="342c1-114">1</span></span>|<span data-ttu-id="342c1-115">Descobrir somente o dispositivo no Exchange que atualizou durante a janela de sincronização delta.</span><span class="sxs-lookup"><span data-stu-id="342c1-115">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|



