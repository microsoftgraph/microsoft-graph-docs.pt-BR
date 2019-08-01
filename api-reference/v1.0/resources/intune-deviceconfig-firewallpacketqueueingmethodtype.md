---
title: tipo de enumeração firewallPacketQueueingMethodType
description: Valores possíveis para firewallPacketQueueingMethod
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 49fdf3172879092a04c20d0d73724744a9ef0fb9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031560"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="1644f-103">tipo de enumeração firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="1644f-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="1644f-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1644f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1644f-105">Valores possíveis para firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="1644f-105">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="1644f-106">Membros</span><span class="sxs-lookup"><span data-stu-id="1644f-106">Members</span></span>
|<span data-ttu-id="1644f-107">Membro</span><span class="sxs-lookup"><span data-stu-id="1644f-107">Member</span></span>|<span data-ttu-id="1644f-108">Valor</span><span class="sxs-lookup"><span data-stu-id="1644f-108">Value</span></span>|<span data-ttu-id="1644f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1644f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1644f-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="1644f-110">deviceDefault</span></span>|<span data-ttu-id="1644f-111">,0</span><span class="sxs-lookup"><span data-stu-id="1644f-111">0</span></span>|<span data-ttu-id="1644f-112">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="1644f-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="1644f-113">deficiência</span><span class="sxs-lookup"><span data-stu-id="1644f-113">disabled</span></span>|<span data-ttu-id="1644f-114">1</span><span class="sxs-lookup"><span data-stu-id="1644f-114">1</span></span>|<span data-ttu-id="1644f-115">Desabilitar enfileiramento de pacotes</span><span class="sxs-lookup"><span data-stu-id="1644f-115">Disable packet queuing</span></span>|
|<span data-ttu-id="1644f-116">queueInbound</span><span class="sxs-lookup"><span data-stu-id="1644f-116">queueInbound</span></span>|<span data-ttu-id="1644f-117">duas</span><span class="sxs-lookup"><span data-stu-id="1644f-117">2</span></span>|<span data-ttu-id="1644f-118">Enfileirar pacotes criptografados de entrada</span><span class="sxs-lookup"><span data-stu-id="1644f-118">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="1644f-119">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="1644f-119">queueOutbound</span></span>|<span data-ttu-id="1644f-120">3D</span><span class="sxs-lookup"><span data-stu-id="1644f-120">3</span></span>|<span data-ttu-id="1644f-121">Pacotes de saída de fila descriptografados para encaminhamento</span><span class="sxs-lookup"><span data-stu-id="1644f-121">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="1644f-122">queueBoth</span><span class="sxs-lookup"><span data-stu-id="1644f-122">queueBoth</span></span>|<span data-ttu-id="1644f-123">quatro</span><span class="sxs-lookup"><span data-stu-id="1644f-123">4</span></span>|<span data-ttu-id="1644f-124">Enfileiramento de pacotes de entrada e de saída</span><span class="sxs-lookup"><span data-stu-id="1644f-124">Queue both inbound and outbound packets</span></span>|



