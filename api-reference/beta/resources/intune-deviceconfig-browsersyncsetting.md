---
title: tipo de enum browserSyncSetting
description: Allow(Not Configured) ou prevent(Block) a sincronização das configurações do navegador de borda da Microsoft. Opção para impedir que está sincronizando entre dispositivos, mas permitir substituição do usuário.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8dce2b82b1eea5e4b06ed0f6949ba6a403b073a8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431230"
---
# <a name="browsersyncsetting-enum-type"></a><span data-ttu-id="38cf5-104">tipo de enum browserSyncSetting</span><span class="sxs-lookup"><span data-stu-id="38cf5-104">browserSyncSetting enum type</span></span>

> <span data-ttu-id="38cf5-105">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="38cf5-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="38cf5-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="38cf5-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="38cf5-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="38cf5-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38cf5-108">Allow(Not Configured) ou prevent(Block) a sincronização das configurações do navegador de borda da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="38cf5-108">Allow(Not Configured) or prevent(Block) the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="38cf5-109">Opção para impedir que está sincronizando entre dispositivos, mas permitir substituição do usuário.</span><span class="sxs-lookup"><span data-stu-id="38cf5-109">Option to prevent syncing across devices, but allow user override.</span></span>

## <a name="members"></a><span data-ttu-id="38cf5-110">Membros</span><span class="sxs-lookup"><span data-stu-id="38cf5-110">Members</span></span>
|<span data-ttu-id="38cf5-111">Membro</span><span class="sxs-lookup"><span data-stu-id="38cf5-111">Member</span></span>|<span data-ttu-id="38cf5-112">Valor</span><span class="sxs-lookup"><span data-stu-id="38cf5-112">Value</span></span>|<span data-ttu-id="38cf5-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="38cf5-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38cf5-114">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="38cf5-114">notConfigured</span></span>|<span data-ttu-id="38cf5-115">0</span><span class="sxs-lookup"><span data-stu-id="38cf5-115">0</span></span>|<span data-ttu-id="38cf5-116">Padrão – permitir entre dispositivos está sincronizando das configurações do navegador.</span><span class="sxs-lookup"><span data-stu-id="38cf5-116">Default – Allow syncing of browser settings across devices.</span></span>|
|<span data-ttu-id="38cf5-117">blockedWithUserOverride</span><span class="sxs-lookup"><span data-stu-id="38cf5-117">blockedWithUserOverride</span></span>|<span data-ttu-id="38cf5-118">1</span><span class="sxs-lookup"><span data-stu-id="38cf5-118">1</span></span>|<span data-ttu-id="38cf5-119">Impedir a sincronização das configurações do navegador entre dispositivos do usuário, Permitir substituição do usuário de configuração.</span><span class="sxs-lookup"><span data-stu-id="38cf5-119">Prevent syncing of browser settings across user devices, allow user override of setting.</span></span>|
|<span data-ttu-id="38cf5-120">bloqueado</span><span class="sxs-lookup"><span data-stu-id="38cf5-120">blocked</span></span>|<span data-ttu-id="38cf5-121">2</span><span class="sxs-lookup"><span data-stu-id="38cf5-121">2</span></span>|<span data-ttu-id="38cf5-122">Absolutamente impedir que está sincronizando das configurações do navegador entre dispositivos do usuário.</span><span class="sxs-lookup"><span data-stu-id="38cf5-122">Absolutely prevent syncing of browser settings across user devices.</span></span>|




