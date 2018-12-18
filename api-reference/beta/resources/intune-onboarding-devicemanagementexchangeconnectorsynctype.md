---
title: tipo de enum deviceManagementExchangeConnectorSyncType
description: O tipo de sincronização do Exchange Connector solicitada.
author: tfitzmac
ms.openlocfilehash: dcad9b1455d488c9243b57f607281b39857cbf25
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316846"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="5d7a4-103">tipo de enum deviceManagementExchangeConnectorSyncType</span><span class="sxs-lookup"><span data-stu-id="5d7a4-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="5d7a4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5d7a4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5d7a4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5d7a4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5d7a4-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5d7a4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5d7a4-107">O tipo de sincronização do Exchange Connector solicitada.</span><span class="sxs-lookup"><span data-stu-id="5d7a4-107">The type of Exchange Connector sync requested.</span></span>
## <a name="members"></a><span data-ttu-id="5d7a4-108">Membros</span><span class="sxs-lookup"><span data-stu-id="5d7a4-108">Members</span></span>
|<span data-ttu-id="5d7a4-109">Membro</span><span class="sxs-lookup"><span data-stu-id="5d7a4-109">Member</span></span>|<span data-ttu-id="5d7a4-110">Valor</span><span class="sxs-lookup"><span data-stu-id="5d7a4-110">Value</span></span>|<span data-ttu-id="5d7a4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d7a4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d7a4-112">fullSync</span><span class="sxs-lookup"><span data-stu-id="5d7a4-112">fullSync</span></span>|<span data-ttu-id="5d7a4-113">0</span><span class="sxs-lookup"><span data-stu-id="5d7a4-113">0</span></span>|<span data-ttu-id="5d7a4-114">Descubra todo o dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="5d7a4-114">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="5d7a4-115">deltaSync</span><span class="sxs-lookup"><span data-stu-id="5d7a4-115">deltaSync</span></span>|<span data-ttu-id="5d7a4-116">1</span><span class="sxs-lookup"><span data-stu-id="5d7a4-116">1</span></span>|<span data-ttu-id="5d7a4-117">Descobrir somente o dispositivo no Exchange que atualizou durante a janela de sincronização delta.</span><span class="sxs-lookup"><span data-stu-id="5d7a4-117">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|





