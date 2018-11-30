---
title: tipo de enum firewallPacketQueueingMethodType
description: Valores possíveis para firewallPacketQueueingMethod
ms.openlocfilehash: f55b68780d3bec97fa48a32c7abd8e1cfb269755
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038270"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="ce47d-103">tipo de enum firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="ce47d-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="ce47d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ce47d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ce47d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ce47d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ce47d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ce47d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ce47d-107">Valores possíveis para firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="ce47d-107">Possible values for firewallPacketQueueingMethod</span></span>
## <a name="members"></a><span data-ttu-id="ce47d-108">Membros</span><span class="sxs-lookup"><span data-stu-id="ce47d-108">Members</span></span>
|<span data-ttu-id="ce47d-109">Membro</span><span class="sxs-lookup"><span data-stu-id="ce47d-109">Member</span></span>|<span data-ttu-id="ce47d-110">Valor</span><span class="sxs-lookup"><span data-stu-id="ce47d-110">Value</span></span>|<span data-ttu-id="ce47d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce47d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce47d-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="ce47d-112">deviceDefault</span></span>|<span data-ttu-id="ce47d-113">0</span><span class="sxs-lookup"><span data-stu-id="ce47d-113">0</span></span>|<span data-ttu-id="ce47d-114">Nenhum valor configurado por Intune, não substituir o valor padrão de dispositivo configurada pelo usuário</span><span class="sxs-lookup"><span data-stu-id="ce47d-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="ce47d-115">desabilitado</span><span class="sxs-lookup"><span data-stu-id="ce47d-115">disabled</span></span>|<span data-ttu-id="ce47d-116">1</span><span class="sxs-lookup"><span data-stu-id="ce47d-116">1</span></span>|<span data-ttu-id="ce47d-117">Desabilitar o serviço de enfileiramento de pacotes</span><span class="sxs-lookup"><span data-stu-id="ce47d-117">Disable packet queuing</span></span>|
|<span data-ttu-id="ce47d-118">queueInbound</span><span class="sxs-lookup"><span data-stu-id="ce47d-118">queueInbound</span></span>|<span data-ttu-id="ce47d-119">2</span><span class="sxs-lookup"><span data-stu-id="ce47d-119">2</span></span>|<span data-ttu-id="ce47d-120">Os pacotes criptografados entrados de fila</span><span class="sxs-lookup"><span data-stu-id="ce47d-120">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="ce47d-121">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="ce47d-121">queueOutbound</span></span>|<span data-ttu-id="ce47d-122">3</span><span class="sxs-lookup"><span data-stu-id="ce47d-122">3</span></span>|<span data-ttu-id="ce47d-123">Fila descriptografados para encaminhamento de pacotes de saída</span><span class="sxs-lookup"><span data-stu-id="ce47d-123">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="ce47d-124">queueBoth</span><span class="sxs-lookup"><span data-stu-id="ce47d-124">queueBoth</span></span>|<span data-ttu-id="ce47d-125">4</span><span class="sxs-lookup"><span data-stu-id="ce47d-125">4</span></span>|<span data-ttu-id="ce47d-126">Pacotes de entrada e saídos da fila</span><span class="sxs-lookup"><span data-stu-id="ce47d-126">Queue both inbound and outbound packets</span></span>|





