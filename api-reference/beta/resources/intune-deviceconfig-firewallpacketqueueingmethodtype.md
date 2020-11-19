---
title: tipo de enumeração firewallPacketQueueingMethodType
description: Valores possíveis para firewallPacketQueueingMethod
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: aca93f0c7afaa0e7859ceccb73fad656f3590b1a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49294449"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="c8b61-103">tipo de enumeração firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="c8b61-103">firewallPacketQueueingMethodType enum type</span></span>

<span data-ttu-id="c8b61-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8b61-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8b61-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c8b61-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8b61-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c8b61-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8b61-107">Valores possíveis para firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="c8b61-107">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="c8b61-108">Membros</span><span class="sxs-lookup"><span data-stu-id="c8b61-108">Members</span></span>
|<span data-ttu-id="c8b61-109">Membro</span><span class="sxs-lookup"><span data-stu-id="c8b61-109">Member</span></span>|<span data-ttu-id="c8b61-110">Valor</span><span class="sxs-lookup"><span data-stu-id="c8b61-110">Value</span></span>|<span data-ttu-id="c8b61-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8b61-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8b61-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="c8b61-112">deviceDefault</span></span>|<span data-ttu-id="c8b61-113">,0</span><span class="sxs-lookup"><span data-stu-id="c8b61-113">0</span></span>|<span data-ttu-id="c8b61-114">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="c8b61-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="c8b61-115">desabilitadas</span><span class="sxs-lookup"><span data-stu-id="c8b61-115">disabled</span></span>|<span data-ttu-id="c8b61-116">1</span><span class="sxs-lookup"><span data-stu-id="c8b61-116">1</span></span>|<span data-ttu-id="c8b61-117">Desabilitar enfileiramento de pacotes</span><span class="sxs-lookup"><span data-stu-id="c8b61-117">Disable packet queuing</span></span>|
|<span data-ttu-id="c8b61-118">queueInbound</span><span class="sxs-lookup"><span data-stu-id="c8b61-118">queueInbound</span></span>|<span data-ttu-id="c8b61-119">duas</span><span class="sxs-lookup"><span data-stu-id="c8b61-119">2</span></span>|<span data-ttu-id="c8b61-120">Enfileirar pacotes criptografados de entrada</span><span class="sxs-lookup"><span data-stu-id="c8b61-120">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="c8b61-121">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="c8b61-121">queueOutbound</span></span>|<span data-ttu-id="c8b61-122">3D</span><span class="sxs-lookup"><span data-stu-id="c8b61-122">3</span></span>|<span data-ttu-id="c8b61-123">Pacotes de saída de fila descriptografados para encaminhamento</span><span class="sxs-lookup"><span data-stu-id="c8b61-123">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="c8b61-124">queueBoth</span><span class="sxs-lookup"><span data-stu-id="c8b61-124">queueBoth</span></span>|<span data-ttu-id="c8b61-125">4 </span><span class="sxs-lookup"><span data-stu-id="c8b61-125">4</span></span>|<span data-ttu-id="c8b61-126">Enfileiramento de pacotes de entrada e de saída</span><span class="sxs-lookup"><span data-stu-id="c8b61-126">Queue both inbound and outbound packets</span></span>|




