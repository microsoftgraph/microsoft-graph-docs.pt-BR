---
title: tipo de enumeração browserSyncSetting
description: Permitir (não configurado) ou impedir (bloquear) a sincronização das configurações do navegador Microsoft Edge. Opção para impedir a sincronização entre dispositivos, mas permitir a substituição do usuário.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: eb478c418c9d5a9dfd971f0bf1732027597679d1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453870"
---
# <a name="browsersyncsetting-enum-type"></a><span data-ttu-id="8cb3d-104">tipo de enumeração browserSyncSetting</span><span class="sxs-lookup"><span data-stu-id="8cb3d-104">browserSyncSetting enum type</span></span>

<span data-ttu-id="8cb3d-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cb3d-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8cb3d-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8cb3d-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8cb3d-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8cb3d-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cb3d-108">Permitir (não configurado) ou impedir (bloquear) a sincronização das configurações do navegador Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="8cb3d-108">Allow(Not Configured) or prevent(Block) the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="8cb3d-109">Opção para impedir a sincronização entre dispositivos, mas permitir a substituição do usuário.</span><span class="sxs-lookup"><span data-stu-id="8cb3d-109">Option to prevent syncing across devices, but allow user override.</span></span>

## <a name="members"></a><span data-ttu-id="8cb3d-110">Membros</span><span class="sxs-lookup"><span data-stu-id="8cb3d-110">Members</span></span>
|<span data-ttu-id="8cb3d-111">Membro</span><span class="sxs-lookup"><span data-stu-id="8cb3d-111">Member</span></span>|<span data-ttu-id="8cb3d-112">Valor</span><span class="sxs-lookup"><span data-stu-id="8cb3d-112">Value</span></span>|<span data-ttu-id="8cb3d-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cb3d-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cb3d-114">notConfigured</span><span class="sxs-lookup"><span data-stu-id="8cb3d-114">notConfigured</span></span>|<span data-ttu-id="8cb3d-115">,0</span><span class="sxs-lookup"><span data-stu-id="8cb3d-115">0</span></span>|<span data-ttu-id="8cb3d-116">Padrão – permite a sincronização de configurações de navegador entre dispositivos.</span><span class="sxs-lookup"><span data-stu-id="8cb3d-116">Default – Allow syncing of browser settings across devices.</span></span>|
|<span data-ttu-id="8cb3d-117">blockedWithUserOverride</span><span class="sxs-lookup"><span data-stu-id="8cb3d-117">blockedWithUserOverride</span></span>|<span data-ttu-id="8cb3d-118">1</span><span class="sxs-lookup"><span data-stu-id="8cb3d-118">1</span></span>|<span data-ttu-id="8cb3d-119">Impedir a sincronização das configurações do navegador nos dispositivos de usuário, permitir a substituição de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="8cb3d-119">Prevent syncing of browser settings across user devices, allow user override of setting.</span></span>|
|<span data-ttu-id="8cb3d-120">bloqueou</span><span class="sxs-lookup"><span data-stu-id="8cb3d-120">blocked</span></span>|<span data-ttu-id="8cb3d-121">duas</span><span class="sxs-lookup"><span data-stu-id="8cb3d-121">2</span></span>|<span data-ttu-id="8cb3d-122">Impede totalmente a sincronização das configurações do navegador nos dispositivos de usuário.</span><span class="sxs-lookup"><span data-stu-id="8cb3d-122">Absolutely prevent syncing of browser settings across user devices.</span></span>|



