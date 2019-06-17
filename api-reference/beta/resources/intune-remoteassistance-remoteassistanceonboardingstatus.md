---
title: tipo de enumeração remoteAssistanceOnboardingStatus
description: O status atual do conector do TeamViewer
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 12a127b053482d87a17cb8c3e5ca4a7191ce32aa
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996271"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a><span data-ttu-id="6f603-103">tipo de enumeração remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="6f603-103">remoteAssistanceOnboardingStatus enum type</span></span>

> <span data-ttu-id="6f603-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6f603-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f603-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6f603-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f603-106">O status atual do conector do TeamViewer</span><span class="sxs-lookup"><span data-stu-id="6f603-106">The current TeamViewer connector status</span></span>

## <a name="members"></a><span data-ttu-id="6f603-107">Membros</span><span class="sxs-lookup"><span data-stu-id="6f603-107">Members</span></span>
|<span data-ttu-id="6f603-108">Membro</span><span class="sxs-lookup"><span data-stu-id="6f603-108">Member</span></span>|<span data-ttu-id="6f603-109">Valor</span><span class="sxs-lookup"><span data-stu-id="6f603-109">Value</span></span>|<span data-ttu-id="6f603-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f603-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f603-111">notOnboarded</span><span class="sxs-lookup"><span data-stu-id="6f603-111">notOnboarded</span></span>|<span data-ttu-id="6f603-112">,0</span><span class="sxs-lookup"><span data-stu-id="6f603-112">0</span></span>|<span data-ttu-id="6f603-113">O status relatado quando não há conector do TeamViewer ativo configurado ou ativo</span><span class="sxs-lookup"><span data-stu-id="6f603-113">The status reported when there is no active TeamViewer connector configured or active</span></span>|
|<span data-ttu-id="6f603-114">integração</span><span class="sxs-lookup"><span data-stu-id="6f603-114">onboarding</span></span>|<span data-ttu-id="6f603-115">1</span><span class="sxs-lookup"><span data-stu-id="6f603-115">1</span></span>|<span data-ttu-id="6f603-116">O status relatado quando o sistema iniciou uma conexão do TeamViewer, mas o serviço ainda não concluiu a confirmação de um conector</span><span class="sxs-lookup"><span data-stu-id="6f603-116">The status reported when the system has initiated a TeamViewer connection, but the service has not yet completed the confirmation of a connector</span></span>|
|<span data-ttu-id="6f603-117">integrado</span><span class="sxs-lookup"><span data-stu-id="6f603-117">onboarded</span></span>|<span data-ttu-id="6f603-118">duas</span><span class="sxs-lookup"><span data-stu-id="6f603-118">2</span></span>|<span data-ttu-id="6f603-119">O status relatado quando o sistema trocava com êxito informações de conta com o TeamViewer e agora pode iniciar sessões de assistência remota com clientes</span><span class="sxs-lookup"><span data-stu-id="6f603-119">The status reported when the system has successfully exchanged account information with TeamViewer and can now initiate remote assistance sessions with clients</span></span>|





