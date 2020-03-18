---
title: tipo de enumeração firewallPacketQueueingMethodType
description: Valores possíveis para firewallPacketQueueingMethod
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8d4bd680061f49b91d9106f455487c72e3e7dbd7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791748"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="d376f-103">tipo de enumeração firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="d376f-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="d376f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d376f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d376f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d376f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d376f-106">Valores possíveis para firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="d376f-106">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="d376f-107">Membros</span><span class="sxs-lookup"><span data-stu-id="d376f-107">Members</span></span>
|<span data-ttu-id="d376f-108">Membro</span><span class="sxs-lookup"><span data-stu-id="d376f-108">Member</span></span>|<span data-ttu-id="d376f-109">Valor</span><span class="sxs-lookup"><span data-stu-id="d376f-109">Value</span></span>|<span data-ttu-id="d376f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d376f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d376f-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="d376f-111">deviceDefault</span></span>|<span data-ttu-id="d376f-112">,0</span><span class="sxs-lookup"><span data-stu-id="d376f-112">0</span></span>|<span data-ttu-id="d376f-113">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="d376f-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="d376f-114">deficiência</span><span class="sxs-lookup"><span data-stu-id="d376f-114">disabled</span></span>|<span data-ttu-id="d376f-115">1</span><span class="sxs-lookup"><span data-stu-id="d376f-115">1</span></span>|<span data-ttu-id="d376f-116">Desabilitar enfileiramento de pacotes</span><span class="sxs-lookup"><span data-stu-id="d376f-116">Disable packet queuing</span></span>|
|<span data-ttu-id="d376f-117">queueInbound</span><span class="sxs-lookup"><span data-stu-id="d376f-117">queueInbound</span></span>|<span data-ttu-id="d376f-118">duas</span><span class="sxs-lookup"><span data-stu-id="d376f-118">2</span></span>|<span data-ttu-id="d376f-119">Enfileirar pacotes criptografados de entrada</span><span class="sxs-lookup"><span data-stu-id="d376f-119">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="d376f-120">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="d376f-120">queueOutbound</span></span>|<span data-ttu-id="d376f-121">3D</span><span class="sxs-lookup"><span data-stu-id="d376f-121">3</span></span>|<span data-ttu-id="d376f-122">Pacotes de saída de fila descriptografados para encaminhamento</span><span class="sxs-lookup"><span data-stu-id="d376f-122">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="d376f-123">queueBoth</span><span class="sxs-lookup"><span data-stu-id="d376f-123">queueBoth</span></span>|<span data-ttu-id="d376f-124">4 </span><span class="sxs-lookup"><span data-stu-id="d376f-124">4</span></span>|<span data-ttu-id="d376f-125">Enfileiramento de pacotes de entrada e de saída</span><span class="sxs-lookup"><span data-stu-id="d376f-125">Queue both inbound and outbound packets</span></span>|



