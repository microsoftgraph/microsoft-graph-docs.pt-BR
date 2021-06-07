---
title: Tipo de número remoteAssistanceOnboardingStatus
description: O status atual do conector teamViewer
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8d63300e02f1442a38bbcda7f8e211e9356b8e57
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755676"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a><span data-ttu-id="da9f8-103">Tipo de número remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="da9f8-103">remoteAssistanceOnboardingStatus enum type</span></span>

<span data-ttu-id="da9f8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da9f8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="da9f8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="da9f8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da9f8-106">O status atual do conector teamViewer</span><span class="sxs-lookup"><span data-stu-id="da9f8-106">The current TeamViewer connector status</span></span>

## <a name="members"></a><span data-ttu-id="da9f8-107">Membros</span><span class="sxs-lookup"><span data-stu-id="da9f8-107">Members</span></span>
|<span data-ttu-id="da9f8-108">Membro</span><span class="sxs-lookup"><span data-stu-id="da9f8-108">Member</span></span>|<span data-ttu-id="da9f8-109">Valor</span><span class="sxs-lookup"><span data-stu-id="da9f8-109">Value</span></span>|<span data-ttu-id="da9f8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="da9f8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da9f8-111">notOnboarded</span><span class="sxs-lookup"><span data-stu-id="da9f8-111">notOnboarded</span></span>|<span data-ttu-id="da9f8-112">0</span><span class="sxs-lookup"><span data-stu-id="da9f8-112">0</span></span>|<span data-ttu-id="da9f8-113">O status relatado quando não há um conector TeamViewer ativo configurado ou ativo</span><span class="sxs-lookup"><span data-stu-id="da9f8-113">The status reported when there is no active TeamViewer connector configured or active</span></span>|
|<span data-ttu-id="da9f8-114">integração</span><span class="sxs-lookup"><span data-stu-id="da9f8-114">onboarding</span></span>|<span data-ttu-id="da9f8-115">1</span><span class="sxs-lookup"><span data-stu-id="da9f8-115">1</span></span>|<span data-ttu-id="da9f8-116">O status relatado quando o sistema iniciou uma conexão TeamViewer, mas o serviço ainda não concluiu a confirmação de um conector</span><span class="sxs-lookup"><span data-stu-id="da9f8-116">The status reported when the system has initiated a TeamViewer connection, but the service has not yet completed the confirmation of a connector</span></span>|
|<span data-ttu-id="da9f8-117">onboarded</span><span class="sxs-lookup"><span data-stu-id="da9f8-117">onboarded</span></span>|<span data-ttu-id="da9f8-118">2</span><span class="sxs-lookup"><span data-stu-id="da9f8-118">2</span></span>|<span data-ttu-id="da9f8-119">O status relatado quando o sistema troca com êxito informações de conta com o TeamViewer e agora pode iniciar sessões de assistência remota com clientes</span><span class="sxs-lookup"><span data-stu-id="da9f8-119">The status reported when the system has successfully exchanged account information with TeamViewer and can now initiate remote assistance sessions with clients</span></span>|




