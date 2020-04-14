---
title: tipo de enumeração configurationManagerClientState
description: Estado do cliente de gerenciador de configurações
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 364a79c23c5f7223accf9828089a9ffd7c0de30a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465012"
---
# <a name="configurationmanagerclientstate-enum-type"></a><span data-ttu-id="a80b9-103">tipo de enumeração configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="a80b9-103">configurationManagerClientState enum type</span></span>

<span data-ttu-id="a80b9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a80b9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a80b9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a80b9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a80b9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a80b9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a80b9-107">Estado do cliente de gerenciador de configurações</span><span class="sxs-lookup"><span data-stu-id="a80b9-107">Configuration manager client state</span></span>

## <a name="members"></a><span data-ttu-id="a80b9-108">Membros</span><span class="sxs-lookup"><span data-stu-id="a80b9-108">Members</span></span>
|<span data-ttu-id="a80b9-109">Membro</span><span class="sxs-lookup"><span data-stu-id="a80b9-109">Member</span></span>|<span data-ttu-id="a80b9-110">Valor</span><span class="sxs-lookup"><span data-stu-id="a80b9-110">Value</span></span>|<span data-ttu-id="a80b9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a80b9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a80b9-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="a80b9-112">unknown</span></span>|<span data-ttu-id="a80b9-113">,0</span><span class="sxs-lookup"><span data-stu-id="a80b9-113">0</span></span>|<span data-ttu-id="a80b9-114">O agente do Gerenciador de configurações é mais antigo que 1806 ou não instalado ou este dispositivo não foi verificado no Intune por mais de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="a80b9-114">Configuration manager agent is older than 1806 or not installed or this device has not checked into Intune for over 30 days.</span></span>|
|<span data-ttu-id="a80b9-115">instalação</span><span class="sxs-lookup"><span data-stu-id="a80b9-115">installed</span></span>|<span data-ttu-id="a80b9-116">1</span><span class="sxs-lookup"><span data-stu-id="a80b9-116">1</span></span>|<span data-ttu-id="a80b9-117">O agente do Gerenciador de configurações está instalado, mas talvez ainda não esteja aparecendo no console do Gerenciador de configurações.</span><span class="sxs-lookup"><span data-stu-id="a80b9-117">The configuration manager agent is installed but may not be showing up in the configuration manager console yet.</span></span> <span data-ttu-id="a80b9-118">Aguarde algumas horas para que ele seja atualizado.</span><span class="sxs-lookup"><span data-stu-id="a80b9-118">Wait a few hours for it to refresh.</span></span>|
|<span data-ttu-id="a80b9-119">condições</span><span class="sxs-lookup"><span data-stu-id="a80b9-119">healthy</span></span>|<span data-ttu-id="a80b9-120">7 </span><span class="sxs-lookup"><span data-stu-id="a80b9-120">7</span></span>|<span data-ttu-id="a80b9-121">Este dispositivo pôde fazer check-in com o serviço do Gerenciador de configurações com êxito.</span><span class="sxs-lookup"><span data-stu-id="a80b9-121">This device was able to check in with the configuration manager service successfully.</span></span>|
|<span data-ttu-id="a80b9-122">installFailed</span><span class="sxs-lookup"><span data-stu-id="a80b9-122">installFailed</span></span>|<span data-ttu-id="a80b9-123">8 </span><span class="sxs-lookup"><span data-stu-id="a80b9-123">8</span></span>|<span data-ttu-id="a80b9-124">Falha ao instalar o agente do Gerenciador de configurações.</span><span class="sxs-lookup"><span data-stu-id="a80b9-124">The configuration manager agent failed to install.</span></span>|
|<span data-ttu-id="a80b9-125">updateFailed</span><span class="sxs-lookup"><span data-stu-id="a80b9-125">updateFailed</span></span>|<span data-ttu-id="a80b9-126">11</span><span class="sxs-lookup"><span data-stu-id="a80b9-126">11</span></span>|<span data-ttu-id="a80b9-127">A atualização da versão x para a versão y do agente do Gerenciador de configuração falhou.</span><span class="sxs-lookup"><span data-stu-id="a80b9-127">The update from version x to version y of the configuration manager agent failed.</span></span> |
|<span data-ttu-id="a80b9-128">communicationError</span><span class="sxs-lookup"><span data-stu-id="a80b9-128">communicationError</span></span>|<span data-ttu-id="a80b9-129">19</span><span class="sxs-lookup"><span data-stu-id="a80b9-129">19</span></span>|<span data-ttu-id="a80b9-130">O agente do Gerenciador de configurações pôde acessar o serviço do Configuration Manager no passado, mas agora não é mais possível.</span><span class="sxs-lookup"><span data-stu-id="a80b9-130">The configuration manager agent was able to reach the configuration manager service in the past but is now no longer able to.</span></span> |



