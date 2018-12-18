---
title: tipo de enum firewallPacketQueueingMethodType
description: Valores possíveis para firewallPacketQueueingMethod
author: tfitzmac
ms.openlocfilehash: 76d8e886c27e7e0e849a4172dbc763013f4cc5ac
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347282"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="3c38a-103">tipo de enum firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="3c38a-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="3c38a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3c38a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c38a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3c38a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3c38a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3c38a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c38a-107">Valores possíveis para firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="3c38a-107">Possible values for firewallPacketQueueingMethod</span></span>
## <a name="members"></a><span data-ttu-id="3c38a-108">Membros</span><span class="sxs-lookup"><span data-stu-id="3c38a-108">Members</span></span>
|<span data-ttu-id="3c38a-109">Membro</span><span class="sxs-lookup"><span data-stu-id="3c38a-109">Member</span></span>|<span data-ttu-id="3c38a-110">Valor</span><span class="sxs-lookup"><span data-stu-id="3c38a-110">Value</span></span>|<span data-ttu-id="3c38a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c38a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c38a-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="3c38a-112">deviceDefault</span></span>|<span data-ttu-id="3c38a-113">0</span><span class="sxs-lookup"><span data-stu-id="3c38a-113">0</span></span>|<span data-ttu-id="3c38a-114">Nenhum valor configurado por Intune, não substituir o valor padrão de dispositivo configurada pelo usuário</span><span class="sxs-lookup"><span data-stu-id="3c38a-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="3c38a-115">desabilitado</span><span class="sxs-lookup"><span data-stu-id="3c38a-115">disabled</span></span>|<span data-ttu-id="3c38a-116">1</span><span class="sxs-lookup"><span data-stu-id="3c38a-116">1</span></span>|<span data-ttu-id="3c38a-117">Desabilitar o serviço de enfileiramento de pacotes</span><span class="sxs-lookup"><span data-stu-id="3c38a-117">Disable packet queuing</span></span>|
|<span data-ttu-id="3c38a-118">queueInbound</span><span class="sxs-lookup"><span data-stu-id="3c38a-118">queueInbound</span></span>|<span data-ttu-id="3c38a-119">2</span><span class="sxs-lookup"><span data-stu-id="3c38a-119">2</span></span>|<span data-ttu-id="3c38a-120">Os pacotes criptografados entrados de fila</span><span class="sxs-lookup"><span data-stu-id="3c38a-120">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="3c38a-121">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="3c38a-121">queueOutbound</span></span>|<span data-ttu-id="3c38a-122">3</span><span class="sxs-lookup"><span data-stu-id="3c38a-122">3</span></span>|<span data-ttu-id="3c38a-123">Fila descriptografados para encaminhamento de pacotes de saída</span><span class="sxs-lookup"><span data-stu-id="3c38a-123">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="3c38a-124">queueBoth</span><span class="sxs-lookup"><span data-stu-id="3c38a-124">queueBoth</span></span>|<span data-ttu-id="3c38a-125">4</span><span class="sxs-lookup"><span data-stu-id="3c38a-125">4</span></span>|<span data-ttu-id="3c38a-126">Pacotes de entrada e saídos da fila</span><span class="sxs-lookup"><span data-stu-id="3c38a-126">Queue both inbound and outbound packets</span></span>|





