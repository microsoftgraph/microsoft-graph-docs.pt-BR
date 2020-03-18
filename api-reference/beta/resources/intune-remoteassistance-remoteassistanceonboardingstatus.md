---
title: tipo de enumeração remoteAssistanceOnboardingStatus
description: O status atual do conector do TeamViewer
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 68e5a8bff7f1753540a2716a00fd9148e188d7ea
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42772934"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a><span data-ttu-id="aa1f9-103">tipo de enumeração remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="aa1f9-103">remoteAssistanceOnboardingStatus enum type</span></span>

> <span data-ttu-id="aa1f9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aa1f9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa1f9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aa1f9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa1f9-106">O status atual do conector do TeamViewer</span><span class="sxs-lookup"><span data-stu-id="aa1f9-106">The current TeamViewer connector status</span></span>

## <a name="members"></a><span data-ttu-id="aa1f9-107">Membros</span><span class="sxs-lookup"><span data-stu-id="aa1f9-107">Members</span></span>
|<span data-ttu-id="aa1f9-108">Membro</span><span class="sxs-lookup"><span data-stu-id="aa1f9-108">Member</span></span>|<span data-ttu-id="aa1f9-109">Valor</span><span class="sxs-lookup"><span data-stu-id="aa1f9-109">Value</span></span>|<span data-ttu-id="aa1f9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa1f9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa1f9-111">notOnboarded</span><span class="sxs-lookup"><span data-stu-id="aa1f9-111">notOnboarded</span></span>|<span data-ttu-id="aa1f9-112">,0</span><span class="sxs-lookup"><span data-stu-id="aa1f9-112">0</span></span>|<span data-ttu-id="aa1f9-113">O status relatado quando não há conector do TeamViewer ativo configurado ou ativo</span><span class="sxs-lookup"><span data-stu-id="aa1f9-113">The status reported when there is no active TeamViewer connector configured or active</span></span>|
|<span data-ttu-id="aa1f9-114">integração</span><span class="sxs-lookup"><span data-stu-id="aa1f9-114">onboarding</span></span>|<span data-ttu-id="aa1f9-115">1</span><span class="sxs-lookup"><span data-stu-id="aa1f9-115">1</span></span>|<span data-ttu-id="aa1f9-116">O status relatado quando o sistema iniciou uma conexão do TeamViewer, mas o serviço ainda não concluiu a confirmação de um conector</span><span class="sxs-lookup"><span data-stu-id="aa1f9-116">The status reported when the system has initiated a TeamViewer connection, but the service has not yet completed the confirmation of a connector</span></span>|
|<span data-ttu-id="aa1f9-117">integrado</span><span class="sxs-lookup"><span data-stu-id="aa1f9-117">onboarded</span></span>|<span data-ttu-id="aa1f9-118">duas</span><span class="sxs-lookup"><span data-stu-id="aa1f9-118">2</span></span>|<span data-ttu-id="aa1f9-119">O status relatado quando o sistema trocava com êxito informações de conta com o TeamViewer e agora pode iniciar sessões de assistência remota com clientes</span><span class="sxs-lookup"><span data-stu-id="aa1f9-119">The status reported when the system has successfully exchanged account information with TeamViewer and can now initiate remote assistance sessions with clients</span></span>|



