---
title: tipo de enumeração firewallPacketQueueingMethodType
description: Valores possíveis para firewallPacketQueueingMethod
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cdd9dc0279abc332bbf7b686f7f429fbd8db8883
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258923"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="3648d-103">tipo de enumeração firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="3648d-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="3648d-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3648d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3648d-105">Valores possíveis para firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="3648d-105">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="3648d-106">Membros</span><span class="sxs-lookup"><span data-stu-id="3648d-106">Members</span></span>
|<span data-ttu-id="3648d-107">Membro</span><span class="sxs-lookup"><span data-stu-id="3648d-107">Member</span></span>|<span data-ttu-id="3648d-108">Valor</span><span class="sxs-lookup"><span data-stu-id="3648d-108">Value</span></span>|<span data-ttu-id="3648d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3648d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3648d-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="3648d-110">deviceDefault</span></span>|<span data-ttu-id="3648d-111">,0</span><span class="sxs-lookup"><span data-stu-id="3648d-111">0</span></span>|<span data-ttu-id="3648d-112">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="3648d-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="3648d-113">deficiência</span><span class="sxs-lookup"><span data-stu-id="3648d-113">disabled</span></span>|<span data-ttu-id="3648d-114">1</span><span class="sxs-lookup"><span data-stu-id="3648d-114">1</span></span>|<span data-ttu-id="3648d-115">Desabilitar enfileiramento de pacotes</span><span class="sxs-lookup"><span data-stu-id="3648d-115">Disable packet queuing</span></span>|
|<span data-ttu-id="3648d-116">queueInbound</span><span class="sxs-lookup"><span data-stu-id="3648d-116">queueInbound</span></span>|<span data-ttu-id="3648d-117">duas</span><span class="sxs-lookup"><span data-stu-id="3648d-117">2</span></span>|<span data-ttu-id="3648d-118">EnFileirar pacotes criptografados de entrada</span><span class="sxs-lookup"><span data-stu-id="3648d-118">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="3648d-119">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="3648d-119">queueOutbound</span></span>|<span data-ttu-id="3648d-120">3D</span><span class="sxs-lookup"><span data-stu-id="3648d-120">3</span></span>|<span data-ttu-id="3648d-121">Pacotes de saída de fila descriptografados para encaminhamento</span><span class="sxs-lookup"><span data-stu-id="3648d-121">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="3648d-122">queueBoth</span><span class="sxs-lookup"><span data-stu-id="3648d-122">queueBoth</span></span>|<span data-ttu-id="3648d-123">quatro</span><span class="sxs-lookup"><span data-stu-id="3648d-123">4</span></span>|<span data-ttu-id="3648d-124">EnFileiramento de pacotes de entrada e de saída</span><span class="sxs-lookup"><span data-stu-id="3648d-124">Queue both inbound and outbound packets</span></span>|



