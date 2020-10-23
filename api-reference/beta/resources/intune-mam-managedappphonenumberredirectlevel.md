---
title: tipo de enumeração managedAppPhoneNumberRedirectLevel
description: As classes de aplicativos que têm permissão para clicar para abrir um número de telefone, para fazer chamadas telefônicas ou enviar mensagens de texto.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1b0e37364bd505dada24d0283477742f70183b83
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722806"
---
# <a name="managedappphonenumberredirectlevel-enum-type"></a><span data-ttu-id="0b1d9-103">tipo de enumeração managedAppPhoneNumberRedirectLevel</span><span class="sxs-lookup"><span data-stu-id="0b1d9-103">managedAppPhoneNumberRedirectLevel enum type</span></span>

<span data-ttu-id="0b1d9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b1d9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0b1d9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0b1d9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b1d9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0b1d9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b1d9-107">As classes de aplicativos que têm permissão para clicar para abrir um número de telefone, para fazer chamadas telefônicas ou enviar mensagens de texto.</span><span class="sxs-lookup"><span data-stu-id="0b1d9-107">The classes of apps that are allowed to click-to-open a phone number, for making phone calls or sending text messages.</span></span>

## <a name="members"></a><span data-ttu-id="0b1d9-108">Membros</span><span class="sxs-lookup"><span data-stu-id="0b1d9-108">Members</span></span>
|<span data-ttu-id="0b1d9-109">Membro</span><span class="sxs-lookup"><span data-stu-id="0b1d9-109">Member</span></span>|<span data-ttu-id="0b1d9-110">Valor</span><span class="sxs-lookup"><span data-stu-id="0b1d9-110">Value</span></span>|<span data-ttu-id="0b1d9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b1d9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b1d9-112">todos os aplicativos</span><span class="sxs-lookup"><span data-stu-id="0b1d9-112">allApps</span></span>|<span data-ttu-id="0b1d9-113">,0</span><span class="sxs-lookup"><span data-stu-id="0b1d9-113">0</span></span>|<span data-ttu-id="0b1d9-114">O compartilhamento é permitido para todos os aplicativos.</span><span class="sxs-lookup"><span data-stu-id="0b1d9-114">Sharing is allowed to all apps.</span></span>|
|<span data-ttu-id="0b1d9-115">managedApps</span><span class="sxs-lookup"><span data-stu-id="0b1d9-115">managedApps</span></span>|<span data-ttu-id="0b1d9-116">1</span><span class="sxs-lookup"><span data-stu-id="0b1d9-116">1</span></span>|<span data-ttu-id="0b1d9-117">O compartilhamento é permitido para todos os aplicativos gerenciados.</span><span class="sxs-lookup"><span data-stu-id="0b1d9-117">Sharing is allowed to all managed apps.</span></span>|
|<span data-ttu-id="0b1d9-118">customApp</span><span class="sxs-lookup"><span data-stu-id="0b1d9-118">customApp</span></span>|<span data-ttu-id="0b1d9-119">duas</span><span class="sxs-lookup"><span data-stu-id="0b1d9-119">2</span></span>|<span data-ttu-id="0b1d9-120">O compartilhamento é permitido para um aplicativo personalizado.</span><span class="sxs-lookup"><span data-stu-id="0b1d9-120">Sharing is allowed to a custom app.</span></span>|
|<span data-ttu-id="0b1d9-121">bloqueou</span><span class="sxs-lookup"><span data-stu-id="0b1d9-121">blocked</span></span>|<span data-ttu-id="0b1d9-122">3D</span><span class="sxs-lookup"><span data-stu-id="0b1d9-122">3</span></span>|<span data-ttu-id="0b1d9-123">O compartilhamento entre aplicativos é bloqueado.</span><span class="sxs-lookup"><span data-stu-id="0b1d9-123">Sharing between apps is blocked.</span></span>|





