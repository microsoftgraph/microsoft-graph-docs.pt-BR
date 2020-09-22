---
title: Gerenciamento de despesas de telecomunicações no Microsoft Intune-API do Microsoft Graph
description: Lista a API do Microsoft Graph para os pontos de extremidade do Intune (REST) relacionadas ao gerenciamento de despesas de telecomunicações para uma organização de locatário.
localization_priority: Normal
author: dougeby
ms.prod: intune
ms.openlocfilehash: c83af322fb8460b4c0a77550213f3ea801f77333
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089347"
---
# <a name="telecom-expense-management-in-microsoft-intune"></a><span data-ttu-id="c522b-103">Gerenciamento de despesas com telecomunicações no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c522b-103">Telecom expense management in Microsoft Intune</span></span>

<span data-ttu-id="c522b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c522b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c522b-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c522b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c522b-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c522b-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c522b-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c522b-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c522b-108">É possível limitar o uso e o roaming de dados em dispositivos de propriedade corporativa ao usar o serviço de gerenciamento de despesas com telecomunicações Saaswedo, que é integrado ao Intune.</span><span class="sxs-lookup"><span data-stu-id="c522b-108">You can limit data usage and roaming on corporate-owned devices when you use the Saaswedo telecom expense management service, which integrates with Intune.</span></span> <span data-ttu-id="c522b-109">O serviço permite configurar e impor limites de uso e enviar aos usuários um alerta quando eles excederem um limite configurado.</span><span class="sxs-lookup"><span data-stu-id="c522b-109">The service enables you to set and enforce usage limits and to send users an alert when they exceed a configured threshold.</span></span> <span data-ttu-id="c522b-110">Também é possível configurar o serviço para realizar outras ações, como a desabilitação do roaming, quando os usuários excederem o limite.</span><span class="sxs-lookup"><span data-stu-id="c522b-110">You can also configure the service to take different actions, such as disabling roaming, when users exceed the threshold.</span></span> <span data-ttu-id="c522b-111">Relatórios com informações sobre o uso e o monitoramento dos dados estão disponíveis no console do Saaswedo.</span><span class="sxs-lookup"><span data-stu-id="c522b-111">Reports that provide data usage and monitoring information are available in the Saaswedo console.</span></span> <span data-ttu-id="c522b-112">Antes de usar o serviço de gerenciamento de despesas com telecomunicações Saaswedo com o Intune, é preciso definir as configurações em um console do Saaswedo e no Intune.</span><span class="sxs-lookup"><span data-stu-id="c522b-112">Before you can use the Saaswedo telecom expense management service with Intune, you need to configure settings in a Saaswedo console and in Intune.</span></span> <span data-ttu-id="c522b-113">A conexão deve ser ativada para o serviço Saaswedo e para o Intune.</span><span class="sxs-lookup"><span data-stu-id="c522b-113">The connection must be turned on for the Saaswedo service and for Intune.</span></span> <span data-ttu-id="c522b-114">Se a conexão do lado do Saaswedo estiver habilitada, mas a do lado do Intune não estiver, o Intune receberá a comunicação, mas ela será ignorada.</span><span class="sxs-lookup"><span data-stu-id="c522b-114">If the Saaswedo side of the connection is enabled, but not the Intune side, Intune receives the communication, but ignores it.</span></span>

<span data-ttu-id="c522b-115">Os seguintes recursos do Graph estão disponíveis para gerenciar despesas com telecomunicações no Intune:</span><span class="sxs-lookup"><span data-stu-id="c522b-115">The following Graph resources are available to manage telecom expenses in Intune:</span></span>

- [<span data-ttu-id="c522b-116">Parceiro de gerenciamento de despesas com telecomunicações</span><span class="sxs-lookup"><span data-stu-id="c522b-116">Telecom expense management partner</span></span>](intune-tem-telecomexpensemanagementpartner.md)



