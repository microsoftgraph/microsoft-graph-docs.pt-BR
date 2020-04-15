---
title: tipo de enumeração firewallPacketQueueingMethodType
description: Valores possíveis para firewallPacketQueueingMethod
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 110fffc41caa4efc6b7fbd9e1efe05f663cf8f85
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447721"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="23522-103">tipo de enumeração firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="23522-103">firewallPacketQueueingMethodType enum type</span></span>

<span data-ttu-id="23522-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23522-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="23522-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="23522-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23522-106">Valores possíveis para firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="23522-106">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="23522-107">Membros</span><span class="sxs-lookup"><span data-stu-id="23522-107">Members</span></span>
|<span data-ttu-id="23522-108">Membro</span><span class="sxs-lookup"><span data-stu-id="23522-108">Member</span></span>|<span data-ttu-id="23522-109">Valor</span><span class="sxs-lookup"><span data-stu-id="23522-109">Value</span></span>|<span data-ttu-id="23522-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="23522-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23522-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="23522-111">deviceDefault</span></span>|<span data-ttu-id="23522-112">,0</span><span class="sxs-lookup"><span data-stu-id="23522-112">0</span></span>|<span data-ttu-id="23522-113">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="23522-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="23522-114">desabilitadas</span><span class="sxs-lookup"><span data-stu-id="23522-114">disabled</span></span>|<span data-ttu-id="23522-115">1</span><span class="sxs-lookup"><span data-stu-id="23522-115">1</span></span>|<span data-ttu-id="23522-116">Desabilitar enfileiramento de pacotes</span><span class="sxs-lookup"><span data-stu-id="23522-116">Disable packet queuing</span></span>|
|<span data-ttu-id="23522-117">queueInbound</span><span class="sxs-lookup"><span data-stu-id="23522-117">queueInbound</span></span>|<span data-ttu-id="23522-118">duas</span><span class="sxs-lookup"><span data-stu-id="23522-118">2</span></span>|<span data-ttu-id="23522-119">Enfileirar pacotes criptografados de entrada</span><span class="sxs-lookup"><span data-stu-id="23522-119">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="23522-120">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="23522-120">queueOutbound</span></span>|<span data-ttu-id="23522-121">3D</span><span class="sxs-lookup"><span data-stu-id="23522-121">3</span></span>|<span data-ttu-id="23522-122">Pacotes de saída de fila descriptografados para encaminhamento</span><span class="sxs-lookup"><span data-stu-id="23522-122">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="23522-123">queueBoth</span><span class="sxs-lookup"><span data-stu-id="23522-123">queueBoth</span></span>|<span data-ttu-id="23522-124">4 </span><span class="sxs-lookup"><span data-stu-id="23522-124">4</span></span>|<span data-ttu-id="23522-125">Enfileiramento de pacotes de entrada e de saída</span><span class="sxs-lookup"><span data-stu-id="23522-125">Queue both inbound and outbound packets</span></span>|







