---
title: tipo de número firewallPacketQueueingMethodType
description: Valores possíveis para firewallPacketQueueingMethod
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a56e30f8b470271ea5fbb91765f7ea6814cbba14
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758852"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="b1775-103">tipo de número firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="b1775-103">firewallPacketQueueingMethodType enum type</span></span>

<span data-ttu-id="b1775-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1775-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1775-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b1775-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1775-106">Valores possíveis para firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="b1775-106">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="b1775-107">Membros</span><span class="sxs-lookup"><span data-stu-id="b1775-107">Members</span></span>
|<span data-ttu-id="b1775-108">Membro</span><span class="sxs-lookup"><span data-stu-id="b1775-108">Member</span></span>|<span data-ttu-id="b1775-109">Valor</span><span class="sxs-lookup"><span data-stu-id="b1775-109">Value</span></span>|<span data-ttu-id="b1775-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1775-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1775-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="b1775-111">deviceDefault</span></span>|<span data-ttu-id="b1775-112">0</span><span class="sxs-lookup"><span data-stu-id="b1775-112">0</span></span>|<span data-ttu-id="b1775-113">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="b1775-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="b1775-114">desabilitadas</span><span class="sxs-lookup"><span data-stu-id="b1775-114">disabled</span></span>|<span data-ttu-id="b1775-115">1</span><span class="sxs-lookup"><span data-stu-id="b1775-115">1</span></span>|<span data-ttu-id="b1775-116">Desabilitar a fila de pacotes</span><span class="sxs-lookup"><span data-stu-id="b1775-116">Disable packet queuing</span></span>|
|<span data-ttu-id="b1775-117">queueInbound</span><span class="sxs-lookup"><span data-stu-id="b1775-117">queueInbound</span></span>|<span data-ttu-id="b1775-118">2</span><span class="sxs-lookup"><span data-stu-id="b1775-118">2</span></span>|<span data-ttu-id="b1775-119">Fila de pacotes criptografados de entrada</span><span class="sxs-lookup"><span data-stu-id="b1775-119">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="b1775-120">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="b1775-120">queueOutbound</span></span>|<span data-ttu-id="b1775-121">3</span><span class="sxs-lookup"><span data-stu-id="b1775-121">3</span></span>|<span data-ttu-id="b1775-122">Pacotes de saída descriptografados da fila para encaminhamento</span><span class="sxs-lookup"><span data-stu-id="b1775-122">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="b1775-123">queueBoth</span><span class="sxs-lookup"><span data-stu-id="b1775-123">queueBoth</span></span>|<span data-ttu-id="b1775-124">4 </span><span class="sxs-lookup"><span data-stu-id="b1775-124">4</span></span>|<span data-ttu-id="b1775-125">Fila de pacotes de entrada e de saída</span><span class="sxs-lookup"><span data-stu-id="b1775-125">Queue both inbound and outbound packets</span></span>|




