---
title: tipo de enum firewallPacketQueueingMethodType
description: Valores possíveis para firewallPacketQueueingMethod
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1303287e521cf0b542047e8acaf122bc08a770a6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823216"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="1caca-103">tipo de enum firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="1caca-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="1caca-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1caca-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1caca-105">Valores possíveis para firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="1caca-105">Possible values for firewallPacketQueueingMethod</span></span>
## <a name="members"></a><span data-ttu-id="1caca-106">Membros</span><span class="sxs-lookup"><span data-stu-id="1caca-106">Members</span></span>
|<span data-ttu-id="1caca-107">Membro</span><span class="sxs-lookup"><span data-stu-id="1caca-107">Member</span></span>|<span data-ttu-id="1caca-108">Valor</span><span class="sxs-lookup"><span data-stu-id="1caca-108">Value</span></span>|<span data-ttu-id="1caca-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1caca-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1caca-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="1caca-110">deviceDefault</span></span>|<span data-ttu-id="1caca-111">0</span><span class="sxs-lookup"><span data-stu-id="1caca-111">0</span></span>|<span data-ttu-id="1caca-112">Nenhum valor configurado por Intune, não substituir o valor padrão de dispositivo configurada pelo usuário</span><span class="sxs-lookup"><span data-stu-id="1caca-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="1caca-113">desabilitado</span><span class="sxs-lookup"><span data-stu-id="1caca-113">disabled</span></span>|<span data-ttu-id="1caca-114">1</span><span class="sxs-lookup"><span data-stu-id="1caca-114">1</span></span>|<span data-ttu-id="1caca-115">Desabilitar o serviço de enfileiramento de pacotes</span><span class="sxs-lookup"><span data-stu-id="1caca-115">Disable packet queuing</span></span>|
|<span data-ttu-id="1caca-116">queueInbound</span><span class="sxs-lookup"><span data-stu-id="1caca-116">queueInbound</span></span>|<span data-ttu-id="1caca-117">2</span><span class="sxs-lookup"><span data-stu-id="1caca-117">2</span></span>|<span data-ttu-id="1caca-118">Os pacotes criptografados entrados de fila</span><span class="sxs-lookup"><span data-stu-id="1caca-118">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="1caca-119">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="1caca-119">queueOutbound</span></span>|<span data-ttu-id="1caca-120">3</span><span class="sxs-lookup"><span data-stu-id="1caca-120">3</span></span>|<span data-ttu-id="1caca-121">Fila descriptografados para encaminhamento de pacotes de saída</span><span class="sxs-lookup"><span data-stu-id="1caca-121">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="1caca-122">queueBoth</span><span class="sxs-lookup"><span data-stu-id="1caca-122">queueBoth</span></span>|<span data-ttu-id="1caca-123">4</span><span class="sxs-lookup"><span data-stu-id="1caca-123">4</span></span>|<span data-ttu-id="1caca-124">Pacotes de entrada e saídos da fila</span><span class="sxs-lookup"><span data-stu-id="1caca-124">Queue both inbound and outbound packets</span></span>|



