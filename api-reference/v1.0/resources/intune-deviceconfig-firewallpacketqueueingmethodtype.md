---
title: tipo de enumeração firewallPacketQueueingMethodType
description: Valores possíveis para firewallPacketQueueingMethod
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c3ed6ebdb4386c8203964ad1072767ec580dce2a
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359226"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="99534-103">tipo de enumeração firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="99534-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="99534-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="99534-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99534-105">Valores possíveis para firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="99534-105">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="99534-106">Membros</span><span class="sxs-lookup"><span data-stu-id="99534-106">Members</span></span>
|<span data-ttu-id="99534-107">Membro</span><span class="sxs-lookup"><span data-stu-id="99534-107">Member</span></span>|<span data-ttu-id="99534-108">Valor</span><span class="sxs-lookup"><span data-stu-id="99534-108">Value</span></span>|<span data-ttu-id="99534-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="99534-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99534-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="99534-110">deviceDefault</span></span>|<span data-ttu-id="99534-111">,0</span><span class="sxs-lookup"><span data-stu-id="99534-111">0</span></span>|<span data-ttu-id="99534-112">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="99534-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="99534-113">deficiência</span><span class="sxs-lookup"><span data-stu-id="99534-113">disabled</span></span>|<span data-ttu-id="99534-114">1</span><span class="sxs-lookup"><span data-stu-id="99534-114">1</span></span>|<span data-ttu-id="99534-115">Desabilitar enfileiramento de pacotes</span><span class="sxs-lookup"><span data-stu-id="99534-115">Disable packet queuing</span></span>|
|<span data-ttu-id="99534-116">queueInbound</span><span class="sxs-lookup"><span data-stu-id="99534-116">queueInbound</span></span>|<span data-ttu-id="99534-117">duas</span><span class="sxs-lookup"><span data-stu-id="99534-117">2</span></span>|<span data-ttu-id="99534-118">Enfileirar pacotes criptografados de entrada</span><span class="sxs-lookup"><span data-stu-id="99534-118">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="99534-119">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="99534-119">queueOutbound</span></span>|<span data-ttu-id="99534-120">3D</span><span class="sxs-lookup"><span data-stu-id="99534-120">3</span></span>|<span data-ttu-id="99534-121">Pacotes de saída de fila descriptografados para encaminhamento</span><span class="sxs-lookup"><span data-stu-id="99534-121">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="99534-122">queueBoth</span><span class="sxs-lookup"><span data-stu-id="99534-122">queueBoth</span></span>|<span data-ttu-id="99534-123">quatro</span><span class="sxs-lookup"><span data-stu-id="99534-123">4</span></span>|<span data-ttu-id="99534-124">Enfileiramento de pacotes de entrada e de saída</span><span class="sxs-lookup"><span data-stu-id="99534-124">Queue both inbound and outbound packets</span></span>|




