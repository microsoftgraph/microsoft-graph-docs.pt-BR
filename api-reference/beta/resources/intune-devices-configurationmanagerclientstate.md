---
title: tipo de enumeração configurationManagerClientState
description: Estado do cliente de gerenciador de configurações
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 74ef4d21529420c4d5bc57bbea5b47ab1bc2baa2
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785046"
---
# <a name="configurationmanagerclientstate-enum-type"></a><span data-ttu-id="6be7f-103">tipo de enumeração configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="6be7f-103">configurationManagerClientState enum type</span></span>

> <span data-ttu-id="6be7f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6be7f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6be7f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6be7f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6be7f-106">Estado do cliente de gerenciador de configurações</span><span class="sxs-lookup"><span data-stu-id="6be7f-106">Configuration manager client state</span></span>

## <a name="members"></a><span data-ttu-id="6be7f-107">Membros</span><span class="sxs-lookup"><span data-stu-id="6be7f-107">Members</span></span>
|<span data-ttu-id="6be7f-108">Membro</span><span class="sxs-lookup"><span data-stu-id="6be7f-108">Member</span></span>|<span data-ttu-id="6be7f-109">Valor</span><span class="sxs-lookup"><span data-stu-id="6be7f-109">Value</span></span>|<span data-ttu-id="6be7f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6be7f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6be7f-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="6be7f-111">unknown</span></span>|<span data-ttu-id="6be7f-112">,0</span><span class="sxs-lookup"><span data-stu-id="6be7f-112">0</span></span>|<span data-ttu-id="6be7f-113">O agente do Gerenciador de configurações é mais antigo que 1806 ou não instalado ou este dispositivo não foi verificado no Intune por mais de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="6be7f-113">Configuration manager agent is older than 1806 or not installed or this device has not checked into Intune for over 30 days.</span></span>|
|<span data-ttu-id="6be7f-114">instalação</span><span class="sxs-lookup"><span data-stu-id="6be7f-114">installed</span></span>|<span data-ttu-id="6be7f-115">1</span><span class="sxs-lookup"><span data-stu-id="6be7f-115">1</span></span>|<span data-ttu-id="6be7f-116">O agente do Gerenciador de configurações está instalado, mas talvez ainda não esteja aparecendo no console do Gerenciador de configurações.</span><span class="sxs-lookup"><span data-stu-id="6be7f-116">The configuration manager agent is installed but may not be showing up in the configuration manager console yet.</span></span> <span data-ttu-id="6be7f-117">Aguarde algumas horas para que ele seja atualizado.</span><span class="sxs-lookup"><span data-stu-id="6be7f-117">Wait a few hours for it to refresh.</span></span>|
|<span data-ttu-id="6be7f-118">condições</span><span class="sxs-lookup"><span data-stu-id="6be7f-118">healthy</span></span>|<span data-ttu-id="6be7f-119">7 </span><span class="sxs-lookup"><span data-stu-id="6be7f-119">7</span></span>|<span data-ttu-id="6be7f-120">Este dispositivo pôde fazer check-in com o serviço do Gerenciador de configurações com êxito.</span><span class="sxs-lookup"><span data-stu-id="6be7f-120">This device was able to check in with the configuration manager service successfully.</span></span>|
|<span data-ttu-id="6be7f-121">installFailed</span><span class="sxs-lookup"><span data-stu-id="6be7f-121">installFailed</span></span>|<span data-ttu-id="6be7f-122">8 </span><span class="sxs-lookup"><span data-stu-id="6be7f-122">8</span></span>|<span data-ttu-id="6be7f-123">Falha ao instalar o agente do Gerenciador de configurações.</span><span class="sxs-lookup"><span data-stu-id="6be7f-123">The configuration manager agent failed to install.</span></span>|
|<span data-ttu-id="6be7f-124">updateFailed</span><span class="sxs-lookup"><span data-stu-id="6be7f-124">updateFailed</span></span>|<span data-ttu-id="6be7f-125">11</span><span class="sxs-lookup"><span data-stu-id="6be7f-125">11</span></span>|<span data-ttu-id="6be7f-126">A atualização da versão x para a versão y do agente do Gerenciador de configuração falhou.</span><span class="sxs-lookup"><span data-stu-id="6be7f-126">The update from version x to version y of the configuration manager agent failed.</span></span> |
|<span data-ttu-id="6be7f-127">communicationError</span><span class="sxs-lookup"><span data-stu-id="6be7f-127">communicationError</span></span>|<span data-ttu-id="6be7f-128">19</span><span class="sxs-lookup"><span data-stu-id="6be7f-128">19</span></span>|<span data-ttu-id="6be7f-129">O agente do Gerenciador de configurações pôde acessar o serviço do Configuration Manager no passado, mas agora não é mais possível.</span><span class="sxs-lookup"><span data-stu-id="6be7f-129">The configuration manager agent was able to reach the configuration manager service in the past but is now no longer able to.</span></span> |



