---
title: tipo de enumeração iosNotificationPreviewVisibility
description: Determina quando as visualizações de notificação são visíveis em um dispositivo iOS. As visualizações podem incluir itens como texto (de mensagens e email) e detalhes do convite (do calendário). Quando configurado, ele substituirá as configurações de visualização definidas pelo usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 607e771ce83858cd22892efa9a377b7997142a24
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301475"
---
# <a name="iosnotificationpreviewvisibility-enum-type"></a><span data-ttu-id="3093a-105">tipo de enumeração iosNotificationPreviewVisibility</span><span class="sxs-lookup"><span data-stu-id="3093a-105">iosNotificationPreviewVisibility enum type</span></span>

<span data-ttu-id="3093a-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3093a-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3093a-107">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3093a-107">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3093a-108">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3093a-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3093a-109">Determina quando as visualizações de notificação são visíveis em um dispositivo iOS.</span><span class="sxs-lookup"><span data-stu-id="3093a-109">Determines when notification previews are visible on an iOS device.</span></span> <span data-ttu-id="3093a-110">As visualizações podem incluir itens como texto (de mensagens e email) e detalhes do convite (do calendário).</span><span class="sxs-lookup"><span data-stu-id="3093a-110">Previews can include things like text (from Messages and Mail) and invitation details (from Calendar).</span></span> <span data-ttu-id="3093a-111">Quando configurado, ele substituirá as configurações de visualização definidas pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="3093a-111">When configured, it will override the user's defined preview settings.</span></span>

## <a name="members"></a><span data-ttu-id="3093a-112">Membros</span><span class="sxs-lookup"><span data-stu-id="3093a-112">Members</span></span>
|<span data-ttu-id="3093a-113">Membro</span><span class="sxs-lookup"><span data-stu-id="3093a-113">Member</span></span>|<span data-ttu-id="3093a-114">Valor</span><span class="sxs-lookup"><span data-stu-id="3093a-114">Value</span></span>|<span data-ttu-id="3093a-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="3093a-115">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3093a-116">notConfigured</span><span class="sxs-lookup"><span data-stu-id="3093a-116">notConfigured</span></span>|<span data-ttu-id="3093a-117">,0</span><span class="sxs-lookup"><span data-stu-id="3093a-117">0</span></span>|<span data-ttu-id="3093a-118">As configurações de visualização de notificação não serão substituídas.</span><span class="sxs-lookup"><span data-stu-id="3093a-118">Notification preview settings will not be overwritten.</span></span>|
|<span data-ttu-id="3093a-119">alwaysShow</span><span class="sxs-lookup"><span data-stu-id="3093a-119">alwaysShow</span></span>|<span data-ttu-id="3093a-120">1</span><span class="sxs-lookup"><span data-stu-id="3093a-120">1</span></span>|<span data-ttu-id="3093a-121">Sempre mostrar visualizações de notificação.</span><span class="sxs-lookup"><span data-stu-id="3093a-121">Always show notification previews.</span></span>|
|<span data-ttu-id="3093a-122">hideWhenLocked</span><span class="sxs-lookup"><span data-stu-id="3093a-122">hideWhenLocked</span></span>|<span data-ttu-id="3093a-123">duas</span><span class="sxs-lookup"><span data-stu-id="3093a-123">2</span></span>|<span data-ttu-id="3093a-124">Mostrar apenas as visualizações de notificação quando o dispositivo estiver desbloqueado.</span><span class="sxs-lookup"><span data-stu-id="3093a-124">Only show notification previews when the device is unlocked.</span></span>|
|<span data-ttu-id="3093a-125">neverShow</span><span class="sxs-lookup"><span data-stu-id="3093a-125">neverShow</span></span>|<span data-ttu-id="3093a-126">3D</span><span class="sxs-lookup"><span data-stu-id="3093a-126">3</span></span>|<span data-ttu-id="3093a-127">Nunca mostrar visualizações de notificação.</span><span class="sxs-lookup"><span data-stu-id="3093a-127">Never show notification previews.</span></span>|




