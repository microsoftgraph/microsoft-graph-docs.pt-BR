---
title: tipo de enumeração configurationManagerClientState
description: Estado do cliente de gerenciador de configurações
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 97fd1dddcfea444d330d3f620244f8f84ebc3da0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000022"
---
# <a name="configurationmanagerclientstate-enum-type"></a><span data-ttu-id="6e457-103">tipo de enumeração configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="6e457-103">configurationManagerClientState enum type</span></span>

> <span data-ttu-id="6e457-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6e457-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e457-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6e457-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e457-106">Estado do cliente de gerenciador de configurações</span><span class="sxs-lookup"><span data-stu-id="6e457-106">Configuration manager client state</span></span>

## <a name="members"></a><span data-ttu-id="6e457-107">Membros</span><span class="sxs-lookup"><span data-stu-id="6e457-107">Members</span></span>
|<span data-ttu-id="6e457-108">Membro</span><span class="sxs-lookup"><span data-stu-id="6e457-108">Member</span></span>|<span data-ttu-id="6e457-109">Valor</span><span class="sxs-lookup"><span data-stu-id="6e457-109">Value</span></span>|<span data-ttu-id="6e457-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e457-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e457-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="6e457-111">unknown</span></span>|<span data-ttu-id="6e457-112">,0</span><span class="sxs-lookup"><span data-stu-id="6e457-112">0</span></span>|<span data-ttu-id="6e457-113">O agente do Gerenciador de configurações é mais antigo que 1806 ou não instalado ou este dispositivo não foi verificado no Intune por mais de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="6e457-113">Configuration manager agent is older than 1806 or not installed or this device has not checked into Intune for over 30 days.</span></span>|
|<span data-ttu-id="6e457-114">instalação</span><span class="sxs-lookup"><span data-stu-id="6e457-114">installed</span></span>|<span data-ttu-id="6e457-115">1</span><span class="sxs-lookup"><span data-stu-id="6e457-115">1</span></span>|<span data-ttu-id="6e457-116">O agente do Gerenciador de configurações está instalado, mas talvez ainda não esteja aparecendo no console do Gerenciador de configurações.</span><span class="sxs-lookup"><span data-stu-id="6e457-116">The configuration manager agent is installed but may not be showing up in the configuration manager console yet.</span></span> <span data-ttu-id="6e457-117">Aguarde algumas horas para que ele seja atualizado.</span><span class="sxs-lookup"><span data-stu-id="6e457-117">Wait a few hours for it to refresh.</span></span>|
|<span data-ttu-id="6e457-118">condições</span><span class="sxs-lookup"><span data-stu-id="6e457-118">healthy</span></span>|<span data-ttu-id="6e457-119">178</span><span class="sxs-lookup"><span data-stu-id="6e457-119">7</span></span>|<span data-ttu-id="6e457-120">Este dispositivo pôde fazer check-in com o serviço do Gerenciador de configurações com êxito.</span><span class="sxs-lookup"><span data-stu-id="6e457-120">This device was able to check in with the configuration manager service successfully.</span></span>|
|<span data-ttu-id="6e457-121">installFailed</span><span class="sxs-lookup"><span data-stu-id="6e457-121">installFailed</span></span>|<span data-ttu-id="6e457-122">8 </span><span class="sxs-lookup"><span data-stu-id="6e457-122">8</span></span>|<span data-ttu-id="6e457-123">Falha ao instalar o agente do Gerenciador de configurações.</span><span class="sxs-lookup"><span data-stu-id="6e457-123">The configuration manager agent failed to install.</span></span>|
|<span data-ttu-id="6e457-124">updateFailed</span><span class="sxs-lookup"><span data-stu-id="6e457-124">updateFailed</span></span>|<span data-ttu-id="6e457-125">11</span><span class="sxs-lookup"><span data-stu-id="6e457-125">11</span></span>|<span data-ttu-id="6e457-126">A atualização da versão x para a versão y do agente do Gerenciador de configuração falhou.</span><span class="sxs-lookup"><span data-stu-id="6e457-126">The update from version x to version y of the configuration manager agent failed.</span></span> |
|<span data-ttu-id="6e457-127">communicationError</span><span class="sxs-lookup"><span data-stu-id="6e457-127">communicationError</span></span>|<span data-ttu-id="6e457-128">19</span><span class="sxs-lookup"><span data-stu-id="6e457-128">19</span></span>|<span data-ttu-id="6e457-129">O agente do Gerenciador de configurações pôde acessar o serviço do Configuration Manager no passado, mas agora não é mais possível.</span><span class="sxs-lookup"><span data-stu-id="6e457-129">The configuration manager agent was able to reach the configuration manager service in the past but is now no longer able to.</span></span> |





