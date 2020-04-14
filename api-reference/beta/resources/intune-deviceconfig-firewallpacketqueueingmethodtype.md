---
title: tipo de enumeração firewallPacketQueueingMethodType
description: Valores possíveis para firewallPacketQueueingMethod
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0a6bd346c45e21c31901d7e54eda95f72fa92a23
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444299"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="47e8c-103">tipo de enumeração firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="47e8c-103">firewallPacketQueueingMethodType enum type</span></span>

<span data-ttu-id="47e8c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47e8c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47e8c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="47e8c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47e8c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="47e8c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47e8c-107">Valores possíveis para firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="47e8c-107">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="47e8c-108">Membros</span><span class="sxs-lookup"><span data-stu-id="47e8c-108">Members</span></span>
|<span data-ttu-id="47e8c-109">Membro</span><span class="sxs-lookup"><span data-stu-id="47e8c-109">Member</span></span>|<span data-ttu-id="47e8c-110">Valor</span><span class="sxs-lookup"><span data-stu-id="47e8c-110">Value</span></span>|<span data-ttu-id="47e8c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="47e8c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47e8c-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="47e8c-112">deviceDefault</span></span>|<span data-ttu-id="47e8c-113">,0</span><span class="sxs-lookup"><span data-stu-id="47e8c-113">0</span></span>|<span data-ttu-id="47e8c-114">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="47e8c-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="47e8c-115">desabilitadas</span><span class="sxs-lookup"><span data-stu-id="47e8c-115">disabled</span></span>|<span data-ttu-id="47e8c-116">1</span><span class="sxs-lookup"><span data-stu-id="47e8c-116">1</span></span>|<span data-ttu-id="47e8c-117">Desabilitar enfileiramento de pacotes</span><span class="sxs-lookup"><span data-stu-id="47e8c-117">Disable packet queuing</span></span>|
|<span data-ttu-id="47e8c-118">queueInbound</span><span class="sxs-lookup"><span data-stu-id="47e8c-118">queueInbound</span></span>|<span data-ttu-id="47e8c-119">duas</span><span class="sxs-lookup"><span data-stu-id="47e8c-119">2</span></span>|<span data-ttu-id="47e8c-120">Enfileirar pacotes criptografados de entrada</span><span class="sxs-lookup"><span data-stu-id="47e8c-120">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="47e8c-121">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="47e8c-121">queueOutbound</span></span>|<span data-ttu-id="47e8c-122">3D</span><span class="sxs-lookup"><span data-stu-id="47e8c-122">3</span></span>|<span data-ttu-id="47e8c-123">Pacotes de saída de fila descriptografados para encaminhamento</span><span class="sxs-lookup"><span data-stu-id="47e8c-123">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="47e8c-124">queueBoth</span><span class="sxs-lookup"><span data-stu-id="47e8c-124">queueBoth</span></span>|<span data-ttu-id="47e8c-125">4 </span><span class="sxs-lookup"><span data-stu-id="47e8c-125">4</span></span>|<span data-ttu-id="47e8c-126">Enfileiramento de pacotes de entrada e de saída</span><span class="sxs-lookup"><span data-stu-id="47e8c-126">Queue both inbound and outbound packets</span></span>|



