---
title: tipo de enumeração browserSyncSetting
description: Permitir (não configurado) ou impedir (bloquear) a sincronização das configurações do navegador Microsoft Edge. Opção para impedir a sincronização entre dispositivos, mas permitir a substituição do usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3bc330373c3578a1bbcf2e6736469c18c926a904
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729823"
---
# <a name="browsersyncsetting-enum-type"></a><span data-ttu-id="f0c54-104">tipo de enumeração browserSyncSetting</span><span class="sxs-lookup"><span data-stu-id="f0c54-104">browserSyncSetting enum type</span></span>

<span data-ttu-id="f0c54-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0c54-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f0c54-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f0c54-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0c54-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f0c54-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0c54-108">Permitir (não configurado) ou impedir (bloquear) a sincronização das configurações do navegador Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="f0c54-108">Allow(Not Configured) or prevent(Block) the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="f0c54-109">Opção para impedir a sincronização entre dispositivos, mas permitir a substituição do usuário.</span><span class="sxs-lookup"><span data-stu-id="f0c54-109">Option to prevent syncing across devices, but allow user override.</span></span>

## <a name="members"></a><span data-ttu-id="f0c54-110">Membros</span><span class="sxs-lookup"><span data-stu-id="f0c54-110">Members</span></span>
|<span data-ttu-id="f0c54-111">Membro</span><span class="sxs-lookup"><span data-stu-id="f0c54-111">Member</span></span>|<span data-ttu-id="f0c54-112">Valor</span><span class="sxs-lookup"><span data-stu-id="f0c54-112">Value</span></span>|<span data-ttu-id="f0c54-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0c54-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0c54-114">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f0c54-114">notConfigured</span></span>|<span data-ttu-id="f0c54-115">,0</span><span class="sxs-lookup"><span data-stu-id="f0c54-115">0</span></span>|<span data-ttu-id="f0c54-116">Padrão – permite a sincronização de configurações de navegador entre dispositivos.</span><span class="sxs-lookup"><span data-stu-id="f0c54-116">Default – Allow syncing of browser settings across devices.</span></span>|
|<span data-ttu-id="f0c54-117">blockedWithUserOverride</span><span class="sxs-lookup"><span data-stu-id="f0c54-117">blockedWithUserOverride</span></span>|<span data-ttu-id="f0c54-118">1</span><span class="sxs-lookup"><span data-stu-id="f0c54-118">1</span></span>|<span data-ttu-id="f0c54-119">Impedir a sincronização das configurações do navegador nos dispositivos de usuário, permitir a substituição de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="f0c54-119">Prevent syncing of browser settings across user devices, allow user override of setting.</span></span>|
|<span data-ttu-id="f0c54-120">bloqueou</span><span class="sxs-lookup"><span data-stu-id="f0c54-120">blocked</span></span>|<span data-ttu-id="f0c54-121">duas</span><span class="sxs-lookup"><span data-stu-id="f0c54-121">2</span></span>|<span data-ttu-id="f0c54-122">Impede totalmente a sincronização das configurações do navegador nos dispositivos de usuário.</span><span class="sxs-lookup"><span data-stu-id="f0c54-122">Absolutely prevent syncing of browser settings across user devices.</span></span>|





