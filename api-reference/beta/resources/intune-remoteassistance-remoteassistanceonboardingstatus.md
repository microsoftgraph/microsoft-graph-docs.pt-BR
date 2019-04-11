---
title: tipo de enumeração remoteAssistanceOnboardingStatus
description: O status atual do conector do TeamViewer
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 23490e61f4134b723cfc066043f132c44c295019
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31787894"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a><span data-ttu-id="e0478-103">tipo de enumeração remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="e0478-103">remoteAssistanceOnboardingStatus enum type</span></span>

> <span data-ttu-id="e0478-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e0478-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0478-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e0478-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0478-106">O status atual do conector do TeamViewer</span><span class="sxs-lookup"><span data-stu-id="e0478-106">The current TeamViewer connector status</span></span>

## <a name="members"></a><span data-ttu-id="e0478-107">Membros</span><span class="sxs-lookup"><span data-stu-id="e0478-107">Members</span></span>
|<span data-ttu-id="e0478-108">Membro</span><span class="sxs-lookup"><span data-stu-id="e0478-108">Member</span></span>|<span data-ttu-id="e0478-109">Valor</span><span class="sxs-lookup"><span data-stu-id="e0478-109">Value</span></span>|<span data-ttu-id="e0478-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0478-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0478-111">notOnboarded</span><span class="sxs-lookup"><span data-stu-id="e0478-111">notOnboarded</span></span>|<span data-ttu-id="e0478-112">,0</span><span class="sxs-lookup"><span data-stu-id="e0478-112">0</span></span>|<span data-ttu-id="e0478-113">O status relatado quando não há conector do TeamViewer ativo configurado ou ativo</span><span class="sxs-lookup"><span data-stu-id="e0478-113">The status reported when there is no active TeamViewer connector configured or active</span></span>|
|<span data-ttu-id="e0478-114">integração</span><span class="sxs-lookup"><span data-stu-id="e0478-114">onboarding</span></span>|<span data-ttu-id="e0478-115">1</span><span class="sxs-lookup"><span data-stu-id="e0478-115">1</span></span>|<span data-ttu-id="e0478-116">O status relatado quando o sistema iniciou uma conexão do TeamViewer, mas o serviço ainda não concluiu a confirmação de um conector</span><span class="sxs-lookup"><span data-stu-id="e0478-116">The status reported when the system has initiated a TeamViewer connection, but the service has not yet completed the confirmation of a connector</span></span>|
|<span data-ttu-id="e0478-117">integrado</span><span class="sxs-lookup"><span data-stu-id="e0478-117">onboarded</span></span>|<span data-ttu-id="e0478-118">duas</span><span class="sxs-lookup"><span data-stu-id="e0478-118">2</span></span>|<span data-ttu-id="e0478-119">O status relatado quando o sistema trocava com êxito informações de conta com o TeamViewer e agora pode iniciar sessões de assistência remota com clientes</span><span class="sxs-lookup"><span data-stu-id="e0478-119">The status reported when the system has successfully exchanged account information with TeamViewer and can now initiate remote assistance sessions with clients</span></span>|





