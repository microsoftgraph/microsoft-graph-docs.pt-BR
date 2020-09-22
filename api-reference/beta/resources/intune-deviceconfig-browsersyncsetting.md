---
title: tipo de enumeração browserSyncSetting
description: Permitir (não configurado) ou impedir (bloquear) a sincronização das configurações do navegador Microsoft Edge. Opção para impedir a sincronização entre dispositivos, mas permitir a substituição do usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 6495134df04ac1b94df605b866862273a5321bc3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016377"
---
# <a name="browsersyncsetting-enum-type"></a><span data-ttu-id="9a53d-104">tipo de enumeração browserSyncSetting</span><span class="sxs-lookup"><span data-stu-id="9a53d-104">browserSyncSetting enum type</span></span>

<span data-ttu-id="9a53d-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a53d-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a53d-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9a53d-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a53d-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9a53d-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a53d-108">Permitir (não configurado) ou impedir (bloquear) a sincronização das configurações do navegador Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="9a53d-108">Allow(Not Configured) or prevent(Block) the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="9a53d-109">Opção para impedir a sincronização entre dispositivos, mas permitir a substituição do usuário.</span><span class="sxs-lookup"><span data-stu-id="9a53d-109">Option to prevent syncing across devices, but allow user override.</span></span>

## <a name="members"></a><span data-ttu-id="9a53d-110">Membros</span><span class="sxs-lookup"><span data-stu-id="9a53d-110">Members</span></span>
|<span data-ttu-id="9a53d-111">Membro</span><span class="sxs-lookup"><span data-stu-id="9a53d-111">Member</span></span>|<span data-ttu-id="9a53d-112">Valor</span><span class="sxs-lookup"><span data-stu-id="9a53d-112">Value</span></span>|<span data-ttu-id="9a53d-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a53d-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a53d-114">notConfigured</span><span class="sxs-lookup"><span data-stu-id="9a53d-114">notConfigured</span></span>|<span data-ttu-id="9a53d-115">,0</span><span class="sxs-lookup"><span data-stu-id="9a53d-115">0</span></span>|<span data-ttu-id="9a53d-116">Padrão – permite a sincronização de configurações de navegador entre dispositivos.</span><span class="sxs-lookup"><span data-stu-id="9a53d-116">Default – Allow syncing of browser settings across devices.</span></span>|
|<span data-ttu-id="9a53d-117">blockedWithUserOverride</span><span class="sxs-lookup"><span data-stu-id="9a53d-117">blockedWithUserOverride</span></span>|<span data-ttu-id="9a53d-118">1 </span><span class="sxs-lookup"><span data-stu-id="9a53d-118">1</span></span>|<span data-ttu-id="9a53d-119">Impedir a sincronização das configurações do navegador nos dispositivos de usuário, permitir a substituição de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="9a53d-119">Prevent syncing of browser settings across user devices, allow user override of setting.</span></span>|
|<span data-ttu-id="9a53d-120">bloqueou</span><span class="sxs-lookup"><span data-stu-id="9a53d-120">blocked</span></span>|<span data-ttu-id="9a53d-121">2 </span><span class="sxs-lookup"><span data-stu-id="9a53d-121">2</span></span>|<span data-ttu-id="9a53d-122">Impede totalmente a sincronização das configurações do navegador nos dispositivos de usuário.</span><span class="sxs-lookup"><span data-stu-id="9a53d-122">Absolutely prevent syncing of browser settings across user devices.</span></span>|






