---
title: tipo de enumeração managedAppPhoneNumberRedirectLevel
description: As classes de aplicativos que têm permissão para clicar para abrir um número de telefone, para fazer chamadas telefônicas ou enviar mensagens de texto.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 12e84e617d74dc73c0234ab1cddfbe004ddc8a6a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302590"
---
# <a name="managedappphonenumberredirectlevel-enum-type"></a><span data-ttu-id="bb675-103">tipo de enumeração managedAppPhoneNumberRedirectLevel</span><span class="sxs-lookup"><span data-stu-id="bb675-103">managedAppPhoneNumberRedirectLevel enum type</span></span>

<span data-ttu-id="bb675-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb675-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb675-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bb675-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb675-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bb675-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb675-107">As classes de aplicativos que têm permissão para clicar para abrir um número de telefone, para fazer chamadas telefônicas ou enviar mensagens de texto.</span><span class="sxs-lookup"><span data-stu-id="bb675-107">The classes of apps that are allowed to click-to-open a phone number, for making phone calls or sending text messages.</span></span>

## <a name="members"></a><span data-ttu-id="bb675-108">Membros</span><span class="sxs-lookup"><span data-stu-id="bb675-108">Members</span></span>
|<span data-ttu-id="bb675-109">Membro</span><span class="sxs-lookup"><span data-stu-id="bb675-109">Member</span></span>|<span data-ttu-id="bb675-110">Valor</span><span class="sxs-lookup"><span data-stu-id="bb675-110">Value</span></span>|<span data-ttu-id="bb675-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb675-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb675-112">todos os aplicativos</span><span class="sxs-lookup"><span data-stu-id="bb675-112">allApps</span></span>|<span data-ttu-id="bb675-113">,0</span><span class="sxs-lookup"><span data-stu-id="bb675-113">0</span></span>|<span data-ttu-id="bb675-114">O compartilhamento é permitido para todos os aplicativos.</span><span class="sxs-lookup"><span data-stu-id="bb675-114">Sharing is allowed to all apps.</span></span>|
|<span data-ttu-id="bb675-115">managedApps</span><span class="sxs-lookup"><span data-stu-id="bb675-115">managedApps</span></span>|<span data-ttu-id="bb675-116">1</span><span class="sxs-lookup"><span data-stu-id="bb675-116">1</span></span>|<span data-ttu-id="bb675-117">O compartilhamento é permitido para todos os aplicativos gerenciados.</span><span class="sxs-lookup"><span data-stu-id="bb675-117">Sharing is allowed to all managed apps.</span></span>|
|<span data-ttu-id="bb675-118">customApp</span><span class="sxs-lookup"><span data-stu-id="bb675-118">customApp</span></span>|<span data-ttu-id="bb675-119">duas</span><span class="sxs-lookup"><span data-stu-id="bb675-119">2</span></span>|<span data-ttu-id="bb675-120">O compartilhamento é permitido para um aplicativo personalizado.</span><span class="sxs-lookup"><span data-stu-id="bb675-120">Sharing is allowed to a custom app.</span></span>|
|<span data-ttu-id="bb675-121">bloqueou</span><span class="sxs-lookup"><span data-stu-id="bb675-121">blocked</span></span>|<span data-ttu-id="bb675-122">3D</span><span class="sxs-lookup"><span data-stu-id="bb675-122">3</span></span>|<span data-ttu-id="bb675-123">O compartilhamento entre aplicativos é bloqueado.</span><span class="sxs-lookup"><span data-stu-id="bb675-123">Sharing between apps is blocked.</span></span>|




