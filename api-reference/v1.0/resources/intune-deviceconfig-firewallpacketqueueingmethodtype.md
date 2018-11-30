---
title: tipo de enum firewallPacketQueueingMethodType
description: Valores possíveis para firewallPacketQueueingMethod
ms.openlocfilehash: 70643e300f1a6cc151edeae849e5ae7c5f977750
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005638"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="b3758-103">tipo de enum firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="b3758-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="b3758-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b3758-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3758-105">Valores possíveis para firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="b3758-105">Possible values for firewallPacketQueueingMethod</span></span>
## <a name="members"></a><span data-ttu-id="b3758-106">Membros</span><span class="sxs-lookup"><span data-stu-id="b3758-106">Members</span></span>
|<span data-ttu-id="b3758-107">Membro</span><span class="sxs-lookup"><span data-stu-id="b3758-107">Member</span></span>|<span data-ttu-id="b3758-108">Valor</span><span class="sxs-lookup"><span data-stu-id="b3758-108">Value</span></span>|<span data-ttu-id="b3758-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3758-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3758-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="b3758-110">deviceDefault</span></span>|<span data-ttu-id="b3758-111">0</span><span class="sxs-lookup"><span data-stu-id="b3758-111">0</span></span>|<span data-ttu-id="b3758-112">Nenhum valor configurado por Intune, não substituir o valor padrão de dispositivo configurada pelo usuário</span><span class="sxs-lookup"><span data-stu-id="b3758-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="b3758-113">desabilitado</span><span class="sxs-lookup"><span data-stu-id="b3758-113">disabled</span></span>|<span data-ttu-id="b3758-114">1</span><span class="sxs-lookup"><span data-stu-id="b3758-114">1</span></span>|<span data-ttu-id="b3758-115">Desabilitar o serviço de enfileiramento de pacotes</span><span class="sxs-lookup"><span data-stu-id="b3758-115">Disable packet queuing</span></span>|
|<span data-ttu-id="b3758-116">queueInbound</span><span class="sxs-lookup"><span data-stu-id="b3758-116">queueInbound</span></span>|<span data-ttu-id="b3758-117">2</span><span class="sxs-lookup"><span data-stu-id="b3758-117">2</span></span>|<span data-ttu-id="b3758-118">Os pacotes criptografados entrados de fila</span><span class="sxs-lookup"><span data-stu-id="b3758-118">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="b3758-119">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="b3758-119">queueOutbound</span></span>|<span data-ttu-id="b3758-120">3</span><span class="sxs-lookup"><span data-stu-id="b3758-120">3</span></span>|<span data-ttu-id="b3758-121">Fila descriptografados para encaminhamento de pacotes de saída</span><span class="sxs-lookup"><span data-stu-id="b3758-121">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="b3758-122">queueBoth</span><span class="sxs-lookup"><span data-stu-id="b3758-122">queueBoth</span></span>|<span data-ttu-id="b3758-123">4</span><span class="sxs-lookup"><span data-stu-id="b3758-123">4</span></span>|<span data-ttu-id="b3758-124">Pacotes de entrada e saídos da fila</span><span class="sxs-lookup"><span data-stu-id="b3758-124">Queue both inbound and outbound packets</span></span>|



