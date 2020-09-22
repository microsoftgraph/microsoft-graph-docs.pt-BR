---
title: tipo de enumeração firewallPacketQueueingMethodType
description: Valores possíveis para firewallPacketQueueingMethod
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0774a8b2fa9e2240366ef7a25edf2db252dafd4d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056699"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="be55e-103">tipo de enumeração firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="be55e-103">firewallPacketQueueingMethodType enum type</span></span>

<span data-ttu-id="be55e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be55e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="be55e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="be55e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be55e-106">Valores possíveis para firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="be55e-106">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="be55e-107">Membros</span><span class="sxs-lookup"><span data-stu-id="be55e-107">Members</span></span>
|<span data-ttu-id="be55e-108">Membro</span><span class="sxs-lookup"><span data-stu-id="be55e-108">Member</span></span>|<span data-ttu-id="be55e-109">Valor</span><span class="sxs-lookup"><span data-stu-id="be55e-109">Value</span></span>|<span data-ttu-id="be55e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="be55e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be55e-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="be55e-111">deviceDefault</span></span>|<span data-ttu-id="be55e-112">,0</span><span class="sxs-lookup"><span data-stu-id="be55e-112">0</span></span>|<span data-ttu-id="be55e-113">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="be55e-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="be55e-114">desabilitadas</span><span class="sxs-lookup"><span data-stu-id="be55e-114">disabled</span></span>|<span data-ttu-id="be55e-115">1 </span><span class="sxs-lookup"><span data-stu-id="be55e-115">1</span></span>|<span data-ttu-id="be55e-116">Desabilitar enfileiramento de pacotes</span><span class="sxs-lookup"><span data-stu-id="be55e-116">Disable packet queuing</span></span>|
|<span data-ttu-id="be55e-117">queueInbound</span><span class="sxs-lookup"><span data-stu-id="be55e-117">queueInbound</span></span>|<span data-ttu-id="be55e-118">2 </span><span class="sxs-lookup"><span data-stu-id="be55e-118">2</span></span>|<span data-ttu-id="be55e-119">Enfileirar pacotes criptografados de entrada</span><span class="sxs-lookup"><span data-stu-id="be55e-119">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="be55e-120">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="be55e-120">queueOutbound</span></span>|<span data-ttu-id="be55e-121">3 </span><span class="sxs-lookup"><span data-stu-id="be55e-121">3</span></span>|<span data-ttu-id="be55e-122">Pacotes de saída de fila descriptografados para encaminhamento</span><span class="sxs-lookup"><span data-stu-id="be55e-122">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="be55e-123">queueBoth</span><span class="sxs-lookup"><span data-stu-id="be55e-123">queueBoth</span></span>|<span data-ttu-id="be55e-124">4 </span><span class="sxs-lookup"><span data-stu-id="be55e-124">4</span></span>|<span data-ttu-id="be55e-125">Enfileiramento de pacotes de entrada e de saída</span><span class="sxs-lookup"><span data-stu-id="be55e-125">Queue both inbound and outbound packets</span></span>|









