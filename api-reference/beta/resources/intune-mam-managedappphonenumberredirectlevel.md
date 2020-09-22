---
title: tipo de enumeração managedAppPhoneNumberRedirectLevel
description: As classes de aplicativos que têm permissão para clicar para abrir um número de telefone, para fazer chamadas telefônicas ou enviar mensagens de texto.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3ba720d9917c1d93e9ce06291adae727fc42281c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030308"
---
# <a name="managedappphonenumberredirectlevel-enum-type"></a><span data-ttu-id="58d81-103">tipo de enumeração managedAppPhoneNumberRedirectLevel</span><span class="sxs-lookup"><span data-stu-id="58d81-103">managedAppPhoneNumberRedirectLevel enum type</span></span>

<span data-ttu-id="58d81-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58d81-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58d81-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="58d81-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58d81-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="58d81-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58d81-107">As classes de aplicativos que têm permissão para clicar para abrir um número de telefone, para fazer chamadas telefônicas ou enviar mensagens de texto.</span><span class="sxs-lookup"><span data-stu-id="58d81-107">The classes of apps that are allowed to click-to-open a phone number, for making phone calls or sending text messages.</span></span>

## <a name="members"></a><span data-ttu-id="58d81-108">Membros</span><span class="sxs-lookup"><span data-stu-id="58d81-108">Members</span></span>
|<span data-ttu-id="58d81-109">Membro</span><span class="sxs-lookup"><span data-stu-id="58d81-109">Member</span></span>|<span data-ttu-id="58d81-110">Valor</span><span class="sxs-lookup"><span data-stu-id="58d81-110">Value</span></span>|<span data-ttu-id="58d81-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="58d81-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58d81-112">todos os aplicativos</span><span class="sxs-lookup"><span data-stu-id="58d81-112">allApps</span></span>|<span data-ttu-id="58d81-113">,0</span><span class="sxs-lookup"><span data-stu-id="58d81-113">0</span></span>|<span data-ttu-id="58d81-114">O compartilhamento é permitido para todos os aplicativos.</span><span class="sxs-lookup"><span data-stu-id="58d81-114">Sharing is allowed to all apps.</span></span>|
|<span data-ttu-id="58d81-115">managedApps</span><span class="sxs-lookup"><span data-stu-id="58d81-115">managedApps</span></span>|<span data-ttu-id="58d81-116">1 </span><span class="sxs-lookup"><span data-stu-id="58d81-116">1</span></span>|<span data-ttu-id="58d81-117">O compartilhamento é permitido para todos os aplicativos gerenciados.</span><span class="sxs-lookup"><span data-stu-id="58d81-117">Sharing is allowed to all managed apps.</span></span>|
|<span data-ttu-id="58d81-118">customApp</span><span class="sxs-lookup"><span data-stu-id="58d81-118">customApp</span></span>|<span data-ttu-id="58d81-119">2 </span><span class="sxs-lookup"><span data-stu-id="58d81-119">2</span></span>|<span data-ttu-id="58d81-120">O compartilhamento é permitido para um aplicativo personalizado.</span><span class="sxs-lookup"><span data-stu-id="58d81-120">Sharing is allowed to a custom app.</span></span>|
|<span data-ttu-id="58d81-121">bloqueou</span><span class="sxs-lookup"><span data-stu-id="58d81-121">blocked</span></span>|<span data-ttu-id="58d81-122">3 </span><span class="sxs-lookup"><span data-stu-id="58d81-122">3</span></span>|<span data-ttu-id="58d81-123">O compartilhamento entre aplicativos é bloqueado.</span><span class="sxs-lookup"><span data-stu-id="58d81-123">Sharing between apps is blocked.</span></span>|






