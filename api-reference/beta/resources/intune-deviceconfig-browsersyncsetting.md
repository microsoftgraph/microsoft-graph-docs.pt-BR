---
title: tipo de enumeração browserSyncSetting
description: Permitir (não configurado) ou impedir (bloquear) a sincronização das configurações do navegador Microsoft Edge. Opção para impedir a sincronização entre dispositivos, mas permitir a substituição do usuário.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 014d1920dac25d5344016ff5bbd1af1ede659f4d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990173"
---
# <a name="browsersyncsetting-enum-type"></a><span data-ttu-id="7b698-104">tipo de enumeração browserSyncSetting</span><span class="sxs-lookup"><span data-stu-id="7b698-104">browserSyncSetting enum type</span></span>

> <span data-ttu-id="7b698-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7b698-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b698-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7b698-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b698-107">Permitir (não configurado) ou impedir (bloquear) a sincronização das configurações do navegador Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="7b698-107">Allow(Not Configured) or prevent(Block) the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="7b698-108">Opção para impedir a sincronização entre dispositivos, mas permitir a substituição do usuário.</span><span class="sxs-lookup"><span data-stu-id="7b698-108">Option to prevent syncing across devices, but allow user override.</span></span>

## <a name="members"></a><span data-ttu-id="7b698-109">Membros</span><span class="sxs-lookup"><span data-stu-id="7b698-109">Members</span></span>
|<span data-ttu-id="7b698-110">Membro</span><span class="sxs-lookup"><span data-stu-id="7b698-110">Member</span></span>|<span data-ttu-id="7b698-111">Valor</span><span class="sxs-lookup"><span data-stu-id="7b698-111">Value</span></span>|<span data-ttu-id="7b698-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b698-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b698-113">notConfigured</span><span class="sxs-lookup"><span data-stu-id="7b698-113">notConfigured</span></span>|<span data-ttu-id="7b698-114">,0</span><span class="sxs-lookup"><span data-stu-id="7b698-114">0</span></span>|<span data-ttu-id="7b698-115">Padrão – permite a sincronização de configurações de navegador entre dispositivos.</span><span class="sxs-lookup"><span data-stu-id="7b698-115">Default – Allow syncing of browser settings across devices.</span></span>|
|<span data-ttu-id="7b698-116">blockedWithUserOverride</span><span class="sxs-lookup"><span data-stu-id="7b698-116">blockedWithUserOverride</span></span>|<span data-ttu-id="7b698-117">1</span><span class="sxs-lookup"><span data-stu-id="7b698-117">1</span></span>|<span data-ttu-id="7b698-118">Impedir a sincronização das configurações do navegador nos dispositivos de usuário, permitir a substituição de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="7b698-118">Prevent syncing of browser settings across user devices, allow user override of setting.</span></span>|
|<span data-ttu-id="7b698-119">bloqueou</span><span class="sxs-lookup"><span data-stu-id="7b698-119">blocked</span></span>|<span data-ttu-id="7b698-120">duas</span><span class="sxs-lookup"><span data-stu-id="7b698-120">2</span></span>|<span data-ttu-id="7b698-121">Impede totalmente a sincronização das configurações do navegador nos dispositivos de usuário.</span><span class="sxs-lookup"><span data-stu-id="7b698-121">Absolutely prevent syncing of browser settings across user devices.</span></span>|





