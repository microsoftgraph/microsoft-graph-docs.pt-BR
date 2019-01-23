---
title: tipo de enum configurationManagerClientState
description: Estado de cliente do Gerenciador de configuração
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 82f4b677001346f9bd32c1bc54bed6e7fbac253d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425782"
---
# <a name="configurationmanagerclientstate-enum-type"></a><span data-ttu-id="61d85-103">tipo de enum configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="61d85-103">configurationManagerClientState enum type</span></span>

> <span data-ttu-id="61d85-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="61d85-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="61d85-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="61d85-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="61d85-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="61d85-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61d85-107">Estado de cliente do Gerenciador de configuração</span><span class="sxs-lookup"><span data-stu-id="61d85-107">Configuration manager client state</span></span>

## <a name="members"></a><span data-ttu-id="61d85-108">Membros</span><span class="sxs-lookup"><span data-stu-id="61d85-108">Members</span></span>
|<span data-ttu-id="61d85-109">Membro</span><span class="sxs-lookup"><span data-stu-id="61d85-109">Member</span></span>|<span data-ttu-id="61d85-110">Valor</span><span class="sxs-lookup"><span data-stu-id="61d85-110">Value</span></span>|<span data-ttu-id="61d85-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="61d85-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61d85-112">unknown</span><span class="sxs-lookup"><span data-stu-id="61d85-112">unknown</span></span>|<span data-ttu-id="61d85-113">0</span><span class="sxs-lookup"><span data-stu-id="61d85-113">0</span></span>|<span data-ttu-id="61d85-114">Agente do Gerenciador de configuração é mais antigo que 1806 ou não está instalado ou este dispositivo não tiver verificado em Intune por mais de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="61d85-114">Configuration manager agent is older than 1806 or not installed or this device has not checked into Intune for over 30 days.</span></span>|
|<span data-ttu-id="61d85-115">instalado</span><span class="sxs-lookup"><span data-stu-id="61d85-115">installed</span></span>|<span data-ttu-id="61d85-116">1</span><span class="sxs-lookup"><span data-stu-id="61d85-116">1</span></span>|<span data-ttu-id="61d85-117">O agente do Gerenciador de configuração está instalado, mas pode não ser aparecendo no console do configuration manager ainda.</span><span class="sxs-lookup"><span data-stu-id="61d85-117">The configuration manager agent is installed but may not be showing up in the configuration manager console yet.</span></span> <span data-ttu-id="61d85-118">Aguarde algumas horas para que ele seja atualizada.</span><span class="sxs-lookup"><span data-stu-id="61d85-118">Wait a few hours for it to refresh.</span></span>|
|<span data-ttu-id="61d85-119">Íntegro</span><span class="sxs-lookup"><span data-stu-id="61d85-119">healthy</span></span>|<span data-ttu-id="61d85-120">7</span><span class="sxs-lookup"><span data-stu-id="61d85-120">7</span></span>|<span data-ttu-id="61d85-121">Este dispositivo foi capaz de check-in com o serviço do Gerenciador de configuração com êxito.</span><span class="sxs-lookup"><span data-stu-id="61d85-121">This device was able to check in with the configuration manager service successfully.</span></span>|
|<span data-ttu-id="61d85-122">installFailed</span><span class="sxs-lookup"><span data-stu-id="61d85-122">installFailed</span></span>|<span data-ttu-id="61d85-123">8</span><span class="sxs-lookup"><span data-stu-id="61d85-123">8</span></span>|<span data-ttu-id="61d85-124">Falha na instalação do agente do Gerenciador de configuração.</span><span class="sxs-lookup"><span data-stu-id="61d85-124">The configuration manager agent failed to install.</span></span>|
|<span data-ttu-id="61d85-125">updateFailed</span><span class="sxs-lookup"><span data-stu-id="61d85-125">updateFailed</span></span>|<span data-ttu-id="61d85-126">11</span><span class="sxs-lookup"><span data-stu-id="61d85-126">11</span></span>|<span data-ttu-id="61d85-127">Falha na atualização da versão x a y da versão do agente do Gerenciador de configuração.</span><span class="sxs-lookup"><span data-stu-id="61d85-127">The update from version x to version y of the configuration manager agent failed.</span></span> |
|<span data-ttu-id="61d85-128">communicationError</span><span class="sxs-lookup"><span data-stu-id="61d85-128">communicationError</span></span>|<span data-ttu-id="61d85-129">19</span><span class="sxs-lookup"><span data-stu-id="61d85-129">19</span></span>|<span data-ttu-id="61d85-130">O agente do Gerenciador de configuração foi capaz de acessar o serviço do Gerenciador de configuração no passado, mas agora não é mais possível.</span><span class="sxs-lookup"><span data-stu-id="61d85-130">The configuration manager agent was able to reach the configuration manager service in the past but is now no longer able to.</span></span> |




