---
title: tipo de enumeração remoteAssistanceOnboardingStatus
description: O status atual do conector do TeamViewer
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 64b8e1f1735890236aed6a9f642d4fa5860e016b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527524"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a><span data-ttu-id="fef2e-103">tipo de enumeração remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="fef2e-103">remoteAssistanceOnboardingStatus enum type</span></span>

<span data-ttu-id="fef2e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fef2e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fef2e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fef2e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fef2e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fef2e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fef2e-107">O status atual do conector do TeamViewer</span><span class="sxs-lookup"><span data-stu-id="fef2e-107">The current TeamViewer connector status</span></span>

## <a name="members"></a><span data-ttu-id="fef2e-108">Membros</span><span class="sxs-lookup"><span data-stu-id="fef2e-108">Members</span></span>
|<span data-ttu-id="fef2e-109">Membro</span><span class="sxs-lookup"><span data-stu-id="fef2e-109">Member</span></span>|<span data-ttu-id="fef2e-110">Valor</span><span class="sxs-lookup"><span data-stu-id="fef2e-110">Value</span></span>|<span data-ttu-id="fef2e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fef2e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fef2e-112">notOnboarded</span><span class="sxs-lookup"><span data-stu-id="fef2e-112">notOnboarded</span></span>|<span data-ttu-id="fef2e-113">,0</span><span class="sxs-lookup"><span data-stu-id="fef2e-113">0</span></span>|<span data-ttu-id="fef2e-114">O status relatado quando não há conector do TeamViewer ativo configurado ou ativo</span><span class="sxs-lookup"><span data-stu-id="fef2e-114">The status reported when there is no active TeamViewer connector configured or active</span></span>|
|<span data-ttu-id="fef2e-115">integração</span><span class="sxs-lookup"><span data-stu-id="fef2e-115">onboarding</span></span>|<span data-ttu-id="fef2e-116">1 </span><span class="sxs-lookup"><span data-stu-id="fef2e-116">1</span></span>|<span data-ttu-id="fef2e-117">O status relatado quando o sistema iniciou uma conexão do TeamViewer, mas o serviço ainda não concluiu a confirmação de um conector</span><span class="sxs-lookup"><span data-stu-id="fef2e-117">The status reported when the system has initiated a TeamViewer connection, but the service has not yet completed the confirmation of a connector</span></span>|
|<span data-ttu-id="fef2e-118">integrado</span><span class="sxs-lookup"><span data-stu-id="fef2e-118">onboarded</span></span>|<span data-ttu-id="fef2e-119">2 </span><span class="sxs-lookup"><span data-stu-id="fef2e-119">2</span></span>|<span data-ttu-id="fef2e-120">O status relatado quando o sistema trocava com êxito informações de conta com o TeamViewer e agora pode iniciar sessões de assistência remota com clientes</span><span class="sxs-lookup"><span data-stu-id="fef2e-120">The status reported when the system has successfully exchanged account information with TeamViewer and can now initiate remote assistance sessions with clients</span></span>|



