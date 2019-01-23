---
title: tipo de enum firewallPacketQueueingMethodType
description: Valores possíveis para firewallPacketQueueingMethod
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dc40b93eebc17b1d1abcd9c317da1ffa538512a5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425754"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="8d805-103">tipo de enum firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="8d805-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="8d805-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="8d805-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8d805-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8d805-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8d805-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="8d805-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d805-107">Valores possíveis para firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="8d805-107">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="8d805-108">Membros</span><span class="sxs-lookup"><span data-stu-id="8d805-108">Members</span></span>
|<span data-ttu-id="8d805-109">Membro</span><span class="sxs-lookup"><span data-stu-id="8d805-109">Member</span></span>|<span data-ttu-id="8d805-110">Valor</span><span class="sxs-lookup"><span data-stu-id="8d805-110">Value</span></span>|<span data-ttu-id="8d805-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d805-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d805-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="8d805-112">deviceDefault</span></span>|<span data-ttu-id="8d805-113">0</span><span class="sxs-lookup"><span data-stu-id="8d805-113">0</span></span>|<span data-ttu-id="8d805-114">Nenhum valor configurado por Intune, não substituir o valor padrão de dispositivo configurada pelo usuário</span><span class="sxs-lookup"><span data-stu-id="8d805-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="8d805-115">desabilitado</span><span class="sxs-lookup"><span data-stu-id="8d805-115">disabled</span></span>|<span data-ttu-id="8d805-116">1</span><span class="sxs-lookup"><span data-stu-id="8d805-116">1</span></span>|<span data-ttu-id="8d805-117">Desabilitar o serviço de enfileiramento de pacotes</span><span class="sxs-lookup"><span data-stu-id="8d805-117">Disable packet queuing</span></span>|
|<span data-ttu-id="8d805-118">queueInbound</span><span class="sxs-lookup"><span data-stu-id="8d805-118">queueInbound</span></span>|<span data-ttu-id="8d805-119">2</span><span class="sxs-lookup"><span data-stu-id="8d805-119">2</span></span>|<span data-ttu-id="8d805-120">Os pacotes criptografados entrados de fila</span><span class="sxs-lookup"><span data-stu-id="8d805-120">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="8d805-121">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="8d805-121">queueOutbound</span></span>|<span data-ttu-id="8d805-122">3</span><span class="sxs-lookup"><span data-stu-id="8d805-122">3</span></span>|<span data-ttu-id="8d805-123">Fila descriptografados para encaminhamento de pacotes de saída</span><span class="sxs-lookup"><span data-stu-id="8d805-123">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="8d805-124">queueBoth</span><span class="sxs-lookup"><span data-stu-id="8d805-124">queueBoth</span></span>|<span data-ttu-id="8d805-125">4</span><span class="sxs-lookup"><span data-stu-id="8d805-125">4</span></span>|<span data-ttu-id="8d805-126">Pacotes de entrada e saídos da fila</span><span class="sxs-lookup"><span data-stu-id="8d805-126">Queue both inbound and outbound packets</span></span>|




