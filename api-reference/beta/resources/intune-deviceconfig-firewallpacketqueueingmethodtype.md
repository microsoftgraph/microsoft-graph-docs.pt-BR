---
title: tipo de enumeração firewallPacketQueueingMethodType
description: Valores possíveis para firewallPacketQueueingMethod
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f2b83aa5d13ac170df1f9f99f8e430d10cdaba3e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460580"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="1f64f-103">tipo de enumeração firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="1f64f-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="1f64f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1f64f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f64f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1f64f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f64f-106">Valores possíveis para firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="1f64f-106">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="1f64f-107">Membros</span><span class="sxs-lookup"><span data-stu-id="1f64f-107">Members</span></span>
|<span data-ttu-id="1f64f-108">Membro</span><span class="sxs-lookup"><span data-stu-id="1f64f-108">Member</span></span>|<span data-ttu-id="1f64f-109">Valor</span><span class="sxs-lookup"><span data-stu-id="1f64f-109">Value</span></span>|<span data-ttu-id="1f64f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f64f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f64f-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="1f64f-111">deviceDefault</span></span>|<span data-ttu-id="1f64f-112">,0</span><span class="sxs-lookup"><span data-stu-id="1f64f-112">0</span></span>|<span data-ttu-id="1f64f-113">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="1f64f-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="1f64f-114">deficiência</span><span class="sxs-lookup"><span data-stu-id="1f64f-114">disabled</span></span>|<span data-ttu-id="1f64f-115">1</span><span class="sxs-lookup"><span data-stu-id="1f64f-115">1</span></span>|<span data-ttu-id="1f64f-116">Desabilitar enfileiramento de pacotes</span><span class="sxs-lookup"><span data-stu-id="1f64f-116">Disable packet queuing</span></span>|
|<span data-ttu-id="1f64f-117">queueInbound</span><span class="sxs-lookup"><span data-stu-id="1f64f-117">queueInbound</span></span>|<span data-ttu-id="1f64f-118">duas</span><span class="sxs-lookup"><span data-stu-id="1f64f-118">2</span></span>|<span data-ttu-id="1f64f-119">EnFileirar pacotes criptografados de entrada</span><span class="sxs-lookup"><span data-stu-id="1f64f-119">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="1f64f-120">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="1f64f-120">queueOutbound</span></span>|<span data-ttu-id="1f64f-121">3D</span><span class="sxs-lookup"><span data-stu-id="1f64f-121">3</span></span>|<span data-ttu-id="1f64f-122">Pacotes de saída de fila descriptografados para encaminhamento</span><span class="sxs-lookup"><span data-stu-id="1f64f-122">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="1f64f-123">queueBoth</span><span class="sxs-lookup"><span data-stu-id="1f64f-123">queueBoth</span></span>|<span data-ttu-id="1f64f-124">quatro</span><span class="sxs-lookup"><span data-stu-id="1f64f-124">4</span></span>|<span data-ttu-id="1f64f-125">EnFileiramento de pacotes de entrada e de saída</span><span class="sxs-lookup"><span data-stu-id="1f64f-125">Queue both inbound and outbound packets</span></span>|





