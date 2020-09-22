---
title: tipo de enumeração remoteAssistanceOnboardingStatus
description: O status atual do conector do TeamViewer
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f070740db5b35f32f1ceb3eabeabcd4d8c3a1c9c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039472"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a><span data-ttu-id="a2ba0-103">tipo de enumeração remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="a2ba0-103">remoteAssistanceOnboardingStatus enum type</span></span>

<span data-ttu-id="a2ba0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2ba0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2ba0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a2ba0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2ba0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a2ba0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2ba0-107">O status atual do conector do TeamViewer</span><span class="sxs-lookup"><span data-stu-id="a2ba0-107">The current TeamViewer connector status</span></span>

## <a name="members"></a><span data-ttu-id="a2ba0-108">Membros</span><span class="sxs-lookup"><span data-stu-id="a2ba0-108">Members</span></span>
|<span data-ttu-id="a2ba0-109">Membro</span><span class="sxs-lookup"><span data-stu-id="a2ba0-109">Member</span></span>|<span data-ttu-id="a2ba0-110">Valor</span><span class="sxs-lookup"><span data-stu-id="a2ba0-110">Value</span></span>|<span data-ttu-id="a2ba0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2ba0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2ba0-112">notOnboarded</span><span class="sxs-lookup"><span data-stu-id="a2ba0-112">notOnboarded</span></span>|<span data-ttu-id="a2ba0-113">,0</span><span class="sxs-lookup"><span data-stu-id="a2ba0-113">0</span></span>|<span data-ttu-id="a2ba0-114">O status relatado quando não há conector do TeamViewer ativo configurado ou ativo</span><span class="sxs-lookup"><span data-stu-id="a2ba0-114">The status reported when there is no active TeamViewer connector configured or active</span></span>|
|<span data-ttu-id="a2ba0-115">integração</span><span class="sxs-lookup"><span data-stu-id="a2ba0-115">onboarding</span></span>|<span data-ttu-id="a2ba0-116">1 </span><span class="sxs-lookup"><span data-stu-id="a2ba0-116">1</span></span>|<span data-ttu-id="a2ba0-117">O status relatado quando o sistema iniciou uma conexão do TeamViewer, mas o serviço ainda não concluiu a confirmação de um conector</span><span class="sxs-lookup"><span data-stu-id="a2ba0-117">The status reported when the system has initiated a TeamViewer connection, but the service has not yet completed the confirmation of a connector</span></span>|
|<span data-ttu-id="a2ba0-118">integrado</span><span class="sxs-lookup"><span data-stu-id="a2ba0-118">onboarded</span></span>|<span data-ttu-id="a2ba0-119">2 </span><span class="sxs-lookup"><span data-stu-id="a2ba0-119">2</span></span>|<span data-ttu-id="a2ba0-120">O status relatado quando o sistema trocava com êxito informações de conta com o TeamViewer e agora pode iniciar sessões de assistência remota com clientes</span><span class="sxs-lookup"><span data-stu-id="a2ba0-120">The status reported when the system has successfully exchanged account information with TeamViewer and can now initiate remote assistance sessions with clients</span></span>|






