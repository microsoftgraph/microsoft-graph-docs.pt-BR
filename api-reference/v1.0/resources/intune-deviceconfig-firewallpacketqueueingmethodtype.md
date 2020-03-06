---
title: tipo de enumeração firewallPacketQueueingMethodType
description: Valores possíveis para firewallPacketQueueingMethod
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0b5976d7ff06620db9958dacdfdd0b8b0c81a191
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530723"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="c6eaf-103">tipo de enumeração firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="c6eaf-103">firewallPacketQueueingMethodType enum type</span></span>

<span data-ttu-id="c6eaf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6eaf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c6eaf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c6eaf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6eaf-106">Valores possíveis para firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="c6eaf-106">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="c6eaf-107">Membros</span><span class="sxs-lookup"><span data-stu-id="c6eaf-107">Members</span></span>
|<span data-ttu-id="c6eaf-108">Membro</span><span class="sxs-lookup"><span data-stu-id="c6eaf-108">Member</span></span>|<span data-ttu-id="c6eaf-109">Valor</span><span class="sxs-lookup"><span data-stu-id="c6eaf-109">Value</span></span>|<span data-ttu-id="c6eaf-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6eaf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6eaf-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="c6eaf-111">deviceDefault</span></span>|<span data-ttu-id="c6eaf-112">,0</span><span class="sxs-lookup"><span data-stu-id="c6eaf-112">0</span></span>|<span data-ttu-id="c6eaf-113">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="c6eaf-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="c6eaf-114">deficiência</span><span class="sxs-lookup"><span data-stu-id="c6eaf-114">disabled</span></span>|<span data-ttu-id="c6eaf-115">1 </span><span class="sxs-lookup"><span data-stu-id="c6eaf-115">1</span></span>|<span data-ttu-id="c6eaf-116">Desabilitar enfileiramento de pacotes</span><span class="sxs-lookup"><span data-stu-id="c6eaf-116">Disable packet queuing</span></span>|
|<span data-ttu-id="c6eaf-117">queueInbound</span><span class="sxs-lookup"><span data-stu-id="c6eaf-117">queueInbound</span></span>|<span data-ttu-id="c6eaf-118">2 </span><span class="sxs-lookup"><span data-stu-id="c6eaf-118">2</span></span>|<span data-ttu-id="c6eaf-119">Enfileirar pacotes criptografados de entrada</span><span class="sxs-lookup"><span data-stu-id="c6eaf-119">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="c6eaf-120">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="c6eaf-120">queueOutbound</span></span>|<span data-ttu-id="c6eaf-121">3 </span><span class="sxs-lookup"><span data-stu-id="c6eaf-121">3</span></span>|<span data-ttu-id="c6eaf-122">Pacotes de saída de fila descriptografados para encaminhamento</span><span class="sxs-lookup"><span data-stu-id="c6eaf-122">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="c6eaf-123">queueBoth</span><span class="sxs-lookup"><span data-stu-id="c6eaf-123">queueBoth</span></span>|<span data-ttu-id="c6eaf-124">4 </span><span class="sxs-lookup"><span data-stu-id="c6eaf-124">4</span></span>|<span data-ttu-id="c6eaf-125">Enfileiramento de pacotes de entrada e de saída</span><span class="sxs-lookup"><span data-stu-id="c6eaf-125">Queue both inbound and outbound packets</span></span>|




