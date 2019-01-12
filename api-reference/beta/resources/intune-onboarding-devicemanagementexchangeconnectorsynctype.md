---
title: tipo de enum deviceManagementExchangeConnectorSyncType
description: O tipo de sincronização do Exchange Connector solicitada.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ac6f54c2a09752df2382ae6b27f9dc9387262acf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912726"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="b9bb3-103">tipo de enum deviceManagementExchangeConnectorSyncType</span><span class="sxs-lookup"><span data-stu-id="b9bb3-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="b9bb3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b9bb3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9bb3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b9bb3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b9bb3-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b9bb3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b9bb3-107">O tipo de sincronização do Exchange Connector solicitada.</span><span class="sxs-lookup"><span data-stu-id="b9bb3-107">The type of Exchange Connector sync requested.</span></span>
## <a name="members"></a><span data-ttu-id="b9bb3-108">Membros</span><span class="sxs-lookup"><span data-stu-id="b9bb3-108">Members</span></span>
|<span data-ttu-id="b9bb3-109">Membro</span><span class="sxs-lookup"><span data-stu-id="b9bb3-109">Member</span></span>|<span data-ttu-id="b9bb3-110">Valor</span><span class="sxs-lookup"><span data-stu-id="b9bb3-110">Value</span></span>|<span data-ttu-id="b9bb3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9bb3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9bb3-112">fullSync</span><span class="sxs-lookup"><span data-stu-id="b9bb3-112">fullSync</span></span>|<span data-ttu-id="b9bb3-113">0</span><span class="sxs-lookup"><span data-stu-id="b9bb3-113">0</span></span>|<span data-ttu-id="b9bb3-114">Descubra todo o dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="b9bb3-114">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="b9bb3-115">deltaSync</span><span class="sxs-lookup"><span data-stu-id="b9bb3-115">deltaSync</span></span>|<span data-ttu-id="b9bb3-116">1</span><span class="sxs-lookup"><span data-stu-id="b9bb3-116">1</span></span>|<span data-ttu-id="b9bb3-117">Descobrir somente o dispositivo no Exchange que atualizou durante a janela de sincronização delta.</span><span class="sxs-lookup"><span data-stu-id="b9bb3-117">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|





