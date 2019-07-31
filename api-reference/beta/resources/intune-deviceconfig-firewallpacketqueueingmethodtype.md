---
title: tipo de enumeração firewallPacketQueueingMethodType
description: Valores possíveis para firewallPacketQueueingMethod
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 52765eedfc7df894be32184a7a5f071ae27552cb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001317"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="d16b4-103">tipo de enumeração firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="d16b4-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="d16b4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d16b4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d16b4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d16b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d16b4-106">Valores possíveis para firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="d16b4-106">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="d16b4-107">Membros</span><span class="sxs-lookup"><span data-stu-id="d16b4-107">Members</span></span>
|<span data-ttu-id="d16b4-108">Membro</span><span class="sxs-lookup"><span data-stu-id="d16b4-108">Member</span></span>|<span data-ttu-id="d16b4-109">Valor</span><span class="sxs-lookup"><span data-stu-id="d16b4-109">Value</span></span>|<span data-ttu-id="d16b4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d16b4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d16b4-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="d16b4-111">deviceDefault</span></span>|<span data-ttu-id="d16b4-112">,0</span><span class="sxs-lookup"><span data-stu-id="d16b4-112">0</span></span>|<span data-ttu-id="d16b4-113">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="d16b4-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="d16b4-114">deficiência</span><span class="sxs-lookup"><span data-stu-id="d16b4-114">disabled</span></span>|<span data-ttu-id="d16b4-115">1</span><span class="sxs-lookup"><span data-stu-id="d16b4-115">1</span></span>|<span data-ttu-id="d16b4-116">Desabilitar enfileiramento de pacotes</span><span class="sxs-lookup"><span data-stu-id="d16b4-116">Disable packet queuing</span></span>|
|<span data-ttu-id="d16b4-117">queueInbound</span><span class="sxs-lookup"><span data-stu-id="d16b4-117">queueInbound</span></span>|<span data-ttu-id="d16b4-118">duas</span><span class="sxs-lookup"><span data-stu-id="d16b4-118">2</span></span>|<span data-ttu-id="d16b4-119">Enfileirar pacotes criptografados de entrada</span><span class="sxs-lookup"><span data-stu-id="d16b4-119">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="d16b4-120">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="d16b4-120">queueOutbound</span></span>|<span data-ttu-id="d16b4-121">3D</span><span class="sxs-lookup"><span data-stu-id="d16b4-121">3</span></span>|<span data-ttu-id="d16b4-122">Pacotes de saída de fila descriptografados para encaminhamento</span><span class="sxs-lookup"><span data-stu-id="d16b4-122">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="d16b4-123">queueBoth</span><span class="sxs-lookup"><span data-stu-id="d16b4-123">queueBoth</span></span>|<span data-ttu-id="d16b4-124">quatro</span><span class="sxs-lookup"><span data-stu-id="d16b4-124">4</span></span>|<span data-ttu-id="d16b4-125">Enfileiramento de pacotes de entrada e de saída</span><span class="sxs-lookup"><span data-stu-id="d16b4-125">Queue both inbound and outbound packets</span></span>|





