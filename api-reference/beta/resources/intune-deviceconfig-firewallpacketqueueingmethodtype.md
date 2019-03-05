---
title: tipo de enumeração firewallPacketQueueingMethodType
description: Valores possíveis para firewallPacketQueueingMethod
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e1b8543df5fa2a50cfdfa56c7cb2d96199ba44e7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172202"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="62c16-103">tipo de enumeração firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="62c16-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="62c16-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="62c16-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62c16-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="62c16-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62c16-106">Valores possíveis para firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="62c16-106">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="62c16-107">Membros</span><span class="sxs-lookup"><span data-stu-id="62c16-107">Members</span></span>
|<span data-ttu-id="62c16-108">Membro</span><span class="sxs-lookup"><span data-stu-id="62c16-108">Member</span></span>|<span data-ttu-id="62c16-109">Valor</span><span class="sxs-lookup"><span data-stu-id="62c16-109">Value</span></span>|<span data-ttu-id="62c16-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="62c16-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62c16-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="62c16-111">deviceDefault</span></span>|<span data-ttu-id="62c16-112">,0</span><span class="sxs-lookup"><span data-stu-id="62c16-112">0</span></span>|<span data-ttu-id="62c16-113">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="62c16-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="62c16-114">deficiência</span><span class="sxs-lookup"><span data-stu-id="62c16-114">disabled</span></span>|<span data-ttu-id="62c16-115">1</span><span class="sxs-lookup"><span data-stu-id="62c16-115">1</span></span>|<span data-ttu-id="62c16-116">Desabilitar enfileiramento de pacotes</span><span class="sxs-lookup"><span data-stu-id="62c16-116">Disable packet queuing</span></span>|
|<span data-ttu-id="62c16-117">queueInbound</span><span class="sxs-lookup"><span data-stu-id="62c16-117">queueInbound</span></span>|<span data-ttu-id="62c16-118">duas</span><span class="sxs-lookup"><span data-stu-id="62c16-118">2</span></span>|<span data-ttu-id="62c16-119">EnFileirar pacotes criptografados de entrada</span><span class="sxs-lookup"><span data-stu-id="62c16-119">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="62c16-120">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="62c16-120">queueOutbound</span></span>|<span data-ttu-id="62c16-121">3D</span><span class="sxs-lookup"><span data-stu-id="62c16-121">3</span></span>|<span data-ttu-id="62c16-122">Pacotes de saída de fila descriptografados para encaminhamento</span><span class="sxs-lookup"><span data-stu-id="62c16-122">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="62c16-123">queueBoth</span><span class="sxs-lookup"><span data-stu-id="62c16-123">queueBoth</span></span>|<span data-ttu-id="62c16-124">quatro</span><span class="sxs-lookup"><span data-stu-id="62c16-124">4</span></span>|<span data-ttu-id="62c16-125">EnFileiramento de pacotes de entrada e de saída</span><span class="sxs-lookup"><span data-stu-id="62c16-125">Queue both inbound and outbound packets</span></span>|




