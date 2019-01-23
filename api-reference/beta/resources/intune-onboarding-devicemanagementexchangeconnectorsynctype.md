---
title: tipo de enum deviceManagementExchangeConnectorSyncType
description: O tipo de sincronização do Exchange Connector solicitada.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2a78bf79990eb16ae6dbc62d4c324b905a79a7f2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405622"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="3b750-103">tipo de enum deviceManagementExchangeConnectorSyncType</span><span class="sxs-lookup"><span data-stu-id="3b750-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="3b750-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="3b750-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3b750-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3b750-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3b750-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="3b750-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b750-107">O tipo de sincronização do Exchange Connector solicitada.</span><span class="sxs-lookup"><span data-stu-id="3b750-107">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="3b750-108">Membros</span><span class="sxs-lookup"><span data-stu-id="3b750-108">Members</span></span>
|<span data-ttu-id="3b750-109">Membro</span><span class="sxs-lookup"><span data-stu-id="3b750-109">Member</span></span>|<span data-ttu-id="3b750-110">Valor</span><span class="sxs-lookup"><span data-stu-id="3b750-110">Value</span></span>|<span data-ttu-id="3b750-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b750-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b750-112">fullSync</span><span class="sxs-lookup"><span data-stu-id="3b750-112">fullSync</span></span>|<span data-ttu-id="3b750-113">0</span><span class="sxs-lookup"><span data-stu-id="3b750-113">0</span></span>|<span data-ttu-id="3b750-114">Descubra todo o dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="3b750-114">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="3b750-115">deltaSync</span><span class="sxs-lookup"><span data-stu-id="3b750-115">deltaSync</span></span>|<span data-ttu-id="3b750-116">1</span><span class="sxs-lookup"><span data-stu-id="3b750-116">1</span></span>|<span data-ttu-id="3b750-117">Descobrir somente o dispositivo no Exchange que atualizou durante a janela de sincronização delta.</span><span class="sxs-lookup"><span data-stu-id="3b750-117">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|




