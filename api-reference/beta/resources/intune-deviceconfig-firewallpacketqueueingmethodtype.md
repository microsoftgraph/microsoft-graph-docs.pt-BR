---
title: tipo de enumeração firewallPacketQueueingMethodType
description: Valores possíveis para firewallPacketQueueingMethod
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9b1802e150460e1e687b8303716a723146e4ca67
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946683"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="dddc8-103">tipo de enumeração firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="dddc8-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="dddc8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dddc8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dddc8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dddc8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dddc8-106">Valores possíveis para firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="dddc8-106">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="dddc8-107">Membros</span><span class="sxs-lookup"><span data-stu-id="dddc8-107">Members</span></span>
|<span data-ttu-id="dddc8-108">Membro</span><span class="sxs-lookup"><span data-stu-id="dddc8-108">Member</span></span>|<span data-ttu-id="dddc8-109">Valor</span><span class="sxs-lookup"><span data-stu-id="dddc8-109">Value</span></span>|<span data-ttu-id="dddc8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="dddc8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dddc8-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="dddc8-111">deviceDefault</span></span>|<span data-ttu-id="dddc8-112">,0</span><span class="sxs-lookup"><span data-stu-id="dddc8-112">0</span></span>|<span data-ttu-id="dddc8-113">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="dddc8-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="dddc8-114">deficiência</span><span class="sxs-lookup"><span data-stu-id="dddc8-114">disabled</span></span>|<span data-ttu-id="dddc8-115">1</span><span class="sxs-lookup"><span data-stu-id="dddc8-115">1</span></span>|<span data-ttu-id="dddc8-116">Desabilitar enfileiramento de pacotes</span><span class="sxs-lookup"><span data-stu-id="dddc8-116">Disable packet queuing</span></span>|
|<span data-ttu-id="dddc8-117">queueInbound</span><span class="sxs-lookup"><span data-stu-id="dddc8-117">queueInbound</span></span>|<span data-ttu-id="dddc8-118">duas</span><span class="sxs-lookup"><span data-stu-id="dddc8-118">2</span></span>|<span data-ttu-id="dddc8-119">Enfileirar pacotes criptografados de entrada</span><span class="sxs-lookup"><span data-stu-id="dddc8-119">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="dddc8-120">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="dddc8-120">queueOutbound</span></span>|<span data-ttu-id="dddc8-121">3D</span><span class="sxs-lookup"><span data-stu-id="dddc8-121">3</span></span>|<span data-ttu-id="dddc8-122">Pacotes de saída de fila descriptografados para encaminhamento</span><span class="sxs-lookup"><span data-stu-id="dddc8-122">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="dddc8-123">queueBoth</span><span class="sxs-lookup"><span data-stu-id="dddc8-123">queueBoth</span></span>|<span data-ttu-id="dddc8-124">quatro</span><span class="sxs-lookup"><span data-stu-id="dddc8-124">4</span></span>|<span data-ttu-id="dddc8-125">Enfileiramento de pacotes de entrada e de saída</span><span class="sxs-lookup"><span data-stu-id="dddc8-125">Queue both inbound and outbound packets</span></span>|




