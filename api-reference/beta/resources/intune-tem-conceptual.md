---
title: Gerenciamento de despesas de telecomunicações no Microsoft Intune-API do Microsoft Graph
description: Lista a API do Microsoft Graph para os pontos de extremidade do Intune (REST) relacionadas ao gerenciamento de despesas de telecomunicações para uma organização de locatário.
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 08582cfe5a041db9cd8b17bfca6fab14c7ae864a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967312"
---
# <a name="telecom-expense-management-in-microsoft-intune"></a><span data-ttu-id="1816b-103">Gerenciamento de despesas com telecomunicações no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="1816b-103">Telecom expense management in Microsoft Intune</span></span>

> <span data-ttu-id="1816b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1816b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1816b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1816b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1816b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1816b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1816b-107">É possível limitar o uso e o roaming de dados em dispositivos de propriedade corporativa ao usar o serviço de gerenciamento de despesas com telecomunicações Saaswedo, que é integrado ao Intune.</span><span class="sxs-lookup"><span data-stu-id="1816b-107">You can limit data usage and roaming on corporate-owned devices when you use the Saaswedo telecom expense management service, which integrates with Intune.</span></span> <span data-ttu-id="1816b-108">O serviço permite configurar e impor limites de uso e enviar aos usuários um alerta quando eles excederem um limite configurado.</span><span class="sxs-lookup"><span data-stu-id="1816b-108">The service enables you to set and enforce usage limits and to send users an alert when they exceed a configured threshold.</span></span> <span data-ttu-id="1816b-109">Também é possível configurar o serviço para realizar outras ações, como a desabilitação do roaming, quando os usuários excederem o limite.</span><span class="sxs-lookup"><span data-stu-id="1816b-109">You can also configure the service to take different actions, such as disabling roaming, when users exceed the threshold.</span></span> <span data-ttu-id="1816b-110">Relatórios com informações sobre o uso e o monitoramento dos dados estão disponíveis no console do Saaswedo.</span><span class="sxs-lookup"><span data-stu-id="1816b-110">Reports that provide data usage and monitoring information are available in the Saaswedo console.</span></span> <span data-ttu-id="1816b-111">Antes de usar o serviço de gerenciamento de despesas com telecomunicações Saaswedo com o Intune, é preciso definir as configurações em um console do Saaswedo e no Intune.</span><span class="sxs-lookup"><span data-stu-id="1816b-111">Before you can use the Saaswedo telecom expense management service with Intune, you need to configure settings in a Saaswedo console and in Intune.</span></span> <span data-ttu-id="1816b-112">A conexão deve ser ativada para o serviço Saaswedo e para o Intune.</span><span class="sxs-lookup"><span data-stu-id="1816b-112">The connection must be turned on for the Saaswedo service and for Intune.</span></span> <span data-ttu-id="1816b-113">Se a conexão do lado do Saaswedo estiver habilitada, mas a do lado do Intune não estiver, o Intune receberá a comunicação, mas ela será ignorada.</span><span class="sxs-lookup"><span data-stu-id="1816b-113">If the Saaswedo side of the connection is enabled, but not the Intune side, Intune receives the communication, but ignores it.</span></span>

<span data-ttu-id="1816b-114">Os seguintes recursos do Graph estão disponíveis para gerenciar despesas com telecomunicações no Intune:</span><span class="sxs-lookup"><span data-stu-id="1816b-114">The following Graph resources are available to manage telecom expenses in Intune:</span></span>

- [<span data-ttu-id="1816b-115">Parceiro de gerenciamento de despesas com telecomunicações</span><span class="sxs-lookup"><span data-stu-id="1816b-115">Telecom expense management partner</span></span>](intune-tem-telecomexpensemanagementpartner.md)
