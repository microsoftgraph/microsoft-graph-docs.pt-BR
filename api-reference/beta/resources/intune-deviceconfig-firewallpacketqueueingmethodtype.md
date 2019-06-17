---
title: tipo de enumeração firewallPacketQueueingMethodType
description: Valores possíveis para firewallPacketQueueingMethod
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a4c7556fb3c37f9bfd564e31744f0e27a4482d6e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34985847"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="b0c09-103">tipo de enumeração firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="b0c09-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="b0c09-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b0c09-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0c09-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b0c09-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0c09-106">Valores possíveis para firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="b0c09-106">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="b0c09-107">Membros</span><span class="sxs-lookup"><span data-stu-id="b0c09-107">Members</span></span>
|<span data-ttu-id="b0c09-108">Membro</span><span class="sxs-lookup"><span data-stu-id="b0c09-108">Member</span></span>|<span data-ttu-id="b0c09-109">Valor</span><span class="sxs-lookup"><span data-stu-id="b0c09-109">Value</span></span>|<span data-ttu-id="b0c09-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0c09-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0c09-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="b0c09-111">deviceDefault</span></span>|<span data-ttu-id="b0c09-112">,0</span><span class="sxs-lookup"><span data-stu-id="b0c09-112">0</span></span>|<span data-ttu-id="b0c09-113">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="b0c09-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="b0c09-114">deficiência</span><span class="sxs-lookup"><span data-stu-id="b0c09-114">disabled</span></span>|<span data-ttu-id="b0c09-115">1</span><span class="sxs-lookup"><span data-stu-id="b0c09-115">1</span></span>|<span data-ttu-id="b0c09-116">Desabilitar enfileiramento de pacotes</span><span class="sxs-lookup"><span data-stu-id="b0c09-116">Disable packet queuing</span></span>|
|<span data-ttu-id="b0c09-117">queueInbound</span><span class="sxs-lookup"><span data-stu-id="b0c09-117">queueInbound</span></span>|<span data-ttu-id="b0c09-118">duas</span><span class="sxs-lookup"><span data-stu-id="b0c09-118">2</span></span>|<span data-ttu-id="b0c09-119">Enfileirar pacotes criptografados de entrada</span><span class="sxs-lookup"><span data-stu-id="b0c09-119">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="b0c09-120">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="b0c09-120">queueOutbound</span></span>|<span data-ttu-id="b0c09-121">3D</span><span class="sxs-lookup"><span data-stu-id="b0c09-121">3</span></span>|<span data-ttu-id="b0c09-122">Pacotes de saída de fila descriptografados para encaminhamento</span><span class="sxs-lookup"><span data-stu-id="b0c09-122">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="b0c09-123">queueBoth</span><span class="sxs-lookup"><span data-stu-id="b0c09-123">queueBoth</span></span>|<span data-ttu-id="b0c09-124">quatro</span><span class="sxs-lookup"><span data-stu-id="b0c09-124">4</span></span>|<span data-ttu-id="b0c09-125">Enfileiramento de pacotes de entrada e de saída</span><span class="sxs-lookup"><span data-stu-id="b0c09-125">Queue both inbound and outbound packets</span></span>|





