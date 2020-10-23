---
title: tipo de enumeração remoteAssistanceOnboardingStatus
description: O status atual do conector do TeamViewer
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4c7c29f9e925084dc46894fadbbf1c68ab17fd7b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723796"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a><span data-ttu-id="4e7bd-103">tipo de enumeração remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="4e7bd-103">remoteAssistanceOnboardingStatus enum type</span></span>

<span data-ttu-id="4e7bd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e7bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e7bd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4e7bd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e7bd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4e7bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e7bd-107">O status atual do conector do TeamViewer</span><span class="sxs-lookup"><span data-stu-id="4e7bd-107">The current TeamViewer connector status</span></span>

## <a name="members"></a><span data-ttu-id="4e7bd-108">Membros</span><span class="sxs-lookup"><span data-stu-id="4e7bd-108">Members</span></span>
|<span data-ttu-id="4e7bd-109">Membro</span><span class="sxs-lookup"><span data-stu-id="4e7bd-109">Member</span></span>|<span data-ttu-id="4e7bd-110">Valor</span><span class="sxs-lookup"><span data-stu-id="4e7bd-110">Value</span></span>|<span data-ttu-id="4e7bd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e7bd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e7bd-112">notOnboarded</span><span class="sxs-lookup"><span data-stu-id="4e7bd-112">notOnboarded</span></span>|<span data-ttu-id="4e7bd-113">,0</span><span class="sxs-lookup"><span data-stu-id="4e7bd-113">0</span></span>|<span data-ttu-id="4e7bd-114">O status relatado quando não há conector do TeamViewer ativo configurado ou ativo</span><span class="sxs-lookup"><span data-stu-id="4e7bd-114">The status reported when there is no active TeamViewer connector configured or active</span></span>|
|<span data-ttu-id="4e7bd-115">integração</span><span class="sxs-lookup"><span data-stu-id="4e7bd-115">onboarding</span></span>|<span data-ttu-id="4e7bd-116">1</span><span class="sxs-lookup"><span data-stu-id="4e7bd-116">1</span></span>|<span data-ttu-id="4e7bd-117">O status relatado quando o sistema iniciou uma conexão do TeamViewer, mas o serviço ainda não concluiu a confirmação de um conector</span><span class="sxs-lookup"><span data-stu-id="4e7bd-117">The status reported when the system has initiated a TeamViewer connection, but the service has not yet completed the confirmation of a connector</span></span>|
|<span data-ttu-id="4e7bd-118">integrado</span><span class="sxs-lookup"><span data-stu-id="4e7bd-118">onboarded</span></span>|<span data-ttu-id="4e7bd-119">duas</span><span class="sxs-lookup"><span data-stu-id="4e7bd-119">2</span></span>|<span data-ttu-id="4e7bd-120">O status relatado quando o sistema trocava com êxito informações de conta com o TeamViewer e agora pode iniciar sessões de assistência remota com clientes</span><span class="sxs-lookup"><span data-stu-id="4e7bd-120">The status reported when the system has successfully exchanged account information with TeamViewer and can now initiate remote assistance sessions with clients</span></span>|





