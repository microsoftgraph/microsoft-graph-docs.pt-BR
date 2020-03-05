---
title: tipo de enumeração firewallPacketQueueingMethodType
description: Valores possíveis para firewallPacketQueueingMethod
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3b134e00e0237e407331f0ea0554c54dcf0d39ad
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529988"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="a6965-103">tipo de enumeração firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="a6965-103">firewallPacketQueueingMethodType enum type</span></span>

<span data-ttu-id="a6965-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a6965-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6965-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a6965-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6965-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a6965-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6965-107">Valores possíveis para firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="a6965-107">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="a6965-108">Membros</span><span class="sxs-lookup"><span data-stu-id="a6965-108">Members</span></span>
|<span data-ttu-id="a6965-109">Membro</span><span class="sxs-lookup"><span data-stu-id="a6965-109">Member</span></span>|<span data-ttu-id="a6965-110">Valor</span><span class="sxs-lookup"><span data-stu-id="a6965-110">Value</span></span>|<span data-ttu-id="a6965-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6965-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6965-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="a6965-112">deviceDefault</span></span>|<span data-ttu-id="a6965-113">,0</span><span class="sxs-lookup"><span data-stu-id="a6965-113">0</span></span>|<span data-ttu-id="a6965-114">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="a6965-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="a6965-115">deficiência</span><span class="sxs-lookup"><span data-stu-id="a6965-115">disabled</span></span>|<span data-ttu-id="a6965-116">1 </span><span class="sxs-lookup"><span data-stu-id="a6965-116">1</span></span>|<span data-ttu-id="a6965-117">Desabilitar enfileiramento de pacotes</span><span class="sxs-lookup"><span data-stu-id="a6965-117">Disable packet queuing</span></span>|
|<span data-ttu-id="a6965-118">queueInbound</span><span class="sxs-lookup"><span data-stu-id="a6965-118">queueInbound</span></span>|<span data-ttu-id="a6965-119">2 </span><span class="sxs-lookup"><span data-stu-id="a6965-119">2</span></span>|<span data-ttu-id="a6965-120">Enfileirar pacotes criptografados de entrada</span><span class="sxs-lookup"><span data-stu-id="a6965-120">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="a6965-121">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="a6965-121">queueOutbound</span></span>|<span data-ttu-id="a6965-122">3 </span><span class="sxs-lookup"><span data-stu-id="a6965-122">3</span></span>|<span data-ttu-id="a6965-123">Pacotes de saída de fila descriptografados para encaminhamento</span><span class="sxs-lookup"><span data-stu-id="a6965-123">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="a6965-124">queueBoth</span><span class="sxs-lookup"><span data-stu-id="a6965-124">queueBoth</span></span>|<span data-ttu-id="a6965-125">4 </span><span class="sxs-lookup"><span data-stu-id="a6965-125">4</span></span>|<span data-ttu-id="a6965-126">Enfileiramento de pacotes de entrada e de saída</span><span class="sxs-lookup"><span data-stu-id="a6965-126">Queue both inbound and outbound packets</span></span>|



