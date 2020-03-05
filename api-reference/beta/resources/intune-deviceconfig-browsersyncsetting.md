---
title: tipo de enumeração browserSyncSetting
description: Permitir (não configurado) ou impedir (bloquear) a sincronização das configurações do navegador Microsoft Edge. Opção para impedir a sincronização entre dispositivos, mas permitir a substituição do usuário.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 55b39f987cb3c2846ead0a1dc1c1f8e0c420399a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527004"
---
# <a name="browsersyncsetting-enum-type"></a><span data-ttu-id="72637-104">tipo de enumeração browserSyncSetting</span><span class="sxs-lookup"><span data-stu-id="72637-104">browserSyncSetting enum type</span></span>

<span data-ttu-id="72637-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="72637-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72637-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="72637-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72637-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="72637-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72637-108">Permitir (não configurado) ou impedir (bloquear) a sincronização das configurações do navegador Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="72637-108">Allow(Not Configured) or prevent(Block) the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="72637-109">Opção para impedir a sincronização entre dispositivos, mas permitir a substituição do usuário.</span><span class="sxs-lookup"><span data-stu-id="72637-109">Option to prevent syncing across devices, but allow user override.</span></span>

## <a name="members"></a><span data-ttu-id="72637-110">Membros</span><span class="sxs-lookup"><span data-stu-id="72637-110">Members</span></span>
|<span data-ttu-id="72637-111">Membro</span><span class="sxs-lookup"><span data-stu-id="72637-111">Member</span></span>|<span data-ttu-id="72637-112">Valor</span><span class="sxs-lookup"><span data-stu-id="72637-112">Value</span></span>|<span data-ttu-id="72637-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="72637-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72637-114">notConfigured</span><span class="sxs-lookup"><span data-stu-id="72637-114">notConfigured</span></span>|<span data-ttu-id="72637-115">,0</span><span class="sxs-lookup"><span data-stu-id="72637-115">0</span></span>|<span data-ttu-id="72637-116">Padrão – permite a sincronização de configurações de navegador entre dispositivos.</span><span class="sxs-lookup"><span data-stu-id="72637-116">Default – Allow syncing of browser settings across devices.</span></span>|
|<span data-ttu-id="72637-117">blockedWithUserOverride</span><span class="sxs-lookup"><span data-stu-id="72637-117">blockedWithUserOverride</span></span>|<span data-ttu-id="72637-118">1 </span><span class="sxs-lookup"><span data-stu-id="72637-118">1</span></span>|<span data-ttu-id="72637-119">Impedir a sincronização das configurações do navegador nos dispositivos de usuário, permitir a substituição de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="72637-119">Prevent syncing of browser settings across user devices, allow user override of setting.</span></span>|
|<span data-ttu-id="72637-120">bloqueou</span><span class="sxs-lookup"><span data-stu-id="72637-120">blocked</span></span>|<span data-ttu-id="72637-121">2 </span><span class="sxs-lookup"><span data-stu-id="72637-121">2</span></span>|<span data-ttu-id="72637-122">Impede totalmente a sincronização das configurações do navegador nos dispositivos de usuário.</span><span class="sxs-lookup"><span data-stu-id="72637-122">Absolutely prevent syncing of browser settings across user devices.</span></span>|



