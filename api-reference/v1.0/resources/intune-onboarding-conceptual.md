---
title: Registrar dispositivos para o gerenciamento no Intune
description: " O registro (BYOD) permite que os usuários inscrevam seus telefones pessoais, tablets ou computadores. O registro de dispositivo de propriedade corporativa (COD) permite cenários de gerenciamento como apagamento remoto, dispositivos compartilhados ou afinidade de usuários em um dispositivo."
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: d8a68ee75a267da062a462c8f015f1832494c5e1
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107743"
---
# <a name="enroll-devices-for-management-in-intune"></a><span data-ttu-id="b78fa-104">Registrar dispositivos para o gerenciamento no Intune</span><span class="sxs-lookup"><span data-stu-id="b78fa-104">Enroll devices for management in Intune</span></span>

<span data-ttu-id="b78fa-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b78fa-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b78fa-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b78fa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="b78fa-107">É possível registrar dispositivos, incluindo computadores Windows, para habilitar o gerenciamento de dispositivo móvel (MDM) com o Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="b78fa-107">You can enroll devices, including Windows PCs, to enable mobile device management (MDM) with Microsoft Intune.</span></span> <span data-ttu-id="b78fa-108">Este tópico descreve as diferentes maneiras de registrar dispositivos móveis no gerenciamento do Intune.</span><span class="sxs-lookup"><span data-stu-id="b78fa-108">This topic describes different ways to enroll mobile devices in Intune management.</span></span> <span data-ttu-id="b78fa-109">A maneira de registrar dispositivos depende do tipo de dispositivo, da propriedade e do nível de gerenciamento necessário.</span><span class="sxs-lookup"><span data-stu-id="b78fa-109">The way you enroll your devices depends on the device type, ownership, and the level of management that's needed.</span></span> <span data-ttu-id="b78fa-110">O registro "Traga seu próprio dispositivo" (BYOD) permite aos usuários registrar seus telefones, computador e tablets pessoais.</span><span class="sxs-lookup"><span data-stu-id="b78fa-110">"Bring your own device" (BYOD) enrollment lets users enroll their personal phones, tablets, or PCs.</span></span> <span data-ttu-id="b78fa-111">O registro de dispositivo de propriedade corporativa (COD) permite cenários de gerenciamento como apagamento remoto, dispositivos compartilhados ou afinidade de usuários em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b78fa-111">Corporate-owned device (COD) enrollment enables management scenarios like remote wipe, shared devices, or user affinity for a device.</span></span>

<span data-ttu-id="b78fa-112">Os seguintes recursos do Graph estão disponíveis para gerenciar registros no Intune:</span><span class="sxs-lookup"><span data-stu-id="b78fa-112">The following Graph resources are available to manage enrollment in Intune:</span></span>  

- [<span data-ttu-id="b78fa-113">Parceiro de gerenciamento de conformidade</span><span class="sxs-lookup"><span data-stu-id="b78fa-113">Compliance management partner</span></span>](intune-onboarding-compliancemanagementpartner.md)
- [<span data-ttu-id="b78fa-114">Atribuição de parceiro de gerenciamento de conformidade</span><span class="sxs-lookup"><span data-stu-id="b78fa-114">Compliance management partner assignment</span></span>](intune-onboarding-compliancemanagementpartnerassignment.md)
- [<span data-ttu-id="b78fa-115">Gerenciamento de aplicativos de dispositivo</span><span class="sxs-lookup"><span data-stu-id="b78fa-115">Device app management</span></span>](intune-onboarding-deviceappmanagement.md)
- [<span data-ttu-id="b78fa-116">Categoria do dispositivo</span><span class="sxs-lookup"><span data-stu-id="b78fa-116">Device category</span></span>](intune-onboarding-devicecategory.md)
- [<span data-ttu-id="b78fa-117">Configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="b78fa-117">Device enrollment configuration</span></span>](intune-onboarding-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="b78fa-118">Configuração de limite do registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="b78fa-118">Device enrollment limit configuration</span></span>](intune-onboarding-deviceenrollmentlimitconfiguration.md)
- [<span data-ttu-id="b78fa-119">Restrição da plataforma de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="b78fa-119">Device enrollment platform restriction</span></span>](intune-onboarding-deviceenrollmentplatformrestriction.md)
- [<span data-ttu-id="b78fa-120">Configuração das restrições da plataforma de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="b78fa-120">Device enrollment platform restrictions configuration</span></span>](intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)
- [<span data-ttu-id="b78fa-121">Configuração do Windows Hello para empresas do registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="b78fa-121">Device enrollment Windows Hello for business configuration</span></span>](intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)
- [<span data-ttu-id="b78fa-122">Gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="b78fa-122">Device management</span></span>](intune-onboarding-devicemanagement.md)
- [<span data-ttu-id="b78fa-123">Conector do Exchange de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="b78fa-123">Device management exchange connector</span></span>](intune-onboarding-devicemanagementexchangeconnector.md)
- [<span data-ttu-id="b78fa-124">Status do conector do Exchange de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="b78fa-124">Device management exchange connector status</span></span>](intune-onboarding-devicemanagementexchangeconnectorstatus.md)
- [<span data-ttu-id="b78fa-125">Tipo de sincronização do conector do Exchange de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="b78fa-125">Device management exchange connector sync type</span></span>](intune-onboarding-devicemanagementexchangeconnectorsynctype.md)
- [<span data-ttu-id="b78fa-126">Tipo de conector do Exchange de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="b78fa-126">Device management exchange connector type</span></span>](intune-onboarding-devicemanagementexchangeconnectortype.md)
- [<span data-ttu-id="b78fa-127">Parceiro de gerenciamento do dispositivo</span><span class="sxs-lookup"><span data-stu-id="b78fa-127">Device management partner</span></span>](intune-onboarding-devicemanagementpartner.md)
- [<span data-ttu-id="b78fa-128">Tipo de aplicativo de parceiro de gerenciamento do dispositivo</span><span class="sxs-lookup"><span data-stu-id="b78fa-128">Device management partner app type</span></span>](intune-onboarding-devicemanagementpartnerapptype.md)
- [<span data-ttu-id="b78fa-129">Estado de locatário de parceiro de gerenciamento do dispositivo</span><span class="sxs-lookup"><span data-stu-id="b78fa-129">Device management partner tenant state</span></span>](intune-onboarding-devicemanagementpartnertenantstate.md)
- [<span data-ttu-id="b78fa-130">Habilitação</span><span class="sxs-lookup"><span data-stu-id="b78fa-130">Enablement</span></span>](intune-onboarding-enablement.md)
- [<span data-ttu-id="b78fa-131">Atribuição de configuração do registro</span><span class="sxs-lookup"><span data-stu-id="b78fa-131">Enrollment configuration assignment</span></span>](intune-onboarding-enrollmentconfigurationassignment.md)
- [<span data-ttu-id="b78fa-132">Marca Intune</span><span class="sxs-lookup"><span data-stu-id="b78fa-132">Intune brand</span></span>](intune-onboarding-intunebrand.md)
- [<span data-ttu-id="b78fa-133">Autoridade MDM</span><span class="sxs-lookup"><span data-stu-id="b78fa-133">MDM authority</span></span>](intune-onboarding-mdmauthority.md)
- [<span data-ttu-id="b78fa-134">Conector de defesa contra ameaças móveis</span><span class="sxs-lookup"><span data-stu-id="b78fa-134">Mobile threat defense connector</span></span>](intune-onboarding-mobilethreatdefenseconnector.md)
- [<span data-ttu-id="b78fa-135">Estado de locatário do parceiro de ameaças móveis</span><span class="sxs-lookup"><span data-stu-id="b78fa-135">Mobile threat partner tenant state</span></span>](intune-onboarding-mobilethreatpartnertenantstate.md)
- [<span data-ttu-id="b78fa-136">Configuração de acesso condicional local</span><span class="sxs-lookup"><span data-stu-id="b78fa-136">On-premises conditional access settings</span></span>](intune-onboarding-onpremisesconditionalaccesssettings.md)
- [<span data-ttu-id="b78fa-137">Organização</span><span class="sxs-lookup"><span data-stu-id="b78fa-137">Organization</span></span>](intune-onboarding-organization.md)
- [<span data-ttu-id="b78fa-138">Cores RGB</span><span class="sxs-lookup"><span data-stu-id="b78fa-138">RGB color</span></span>](intune-onboarding-rgbcolor.md)
- [<span data-ttu-id="b78fa-139">Usuário</span><span class="sxs-lookup"><span data-stu-id="b78fa-139">User</span></span>](intune-onboarding-user.md)
- [<span data-ttu-id="b78fa-140">Token VPP</span><span class="sxs-lookup"><span data-stu-id="b78fa-140">VPP token</span></span>](intune-onboarding-vpptoken.md)
- [<span data-ttu-id="b78fa-141">Estado do token VPP</span><span class="sxs-lookup"><span data-stu-id="b78fa-141">VPP token state</span></span>](intune-onboarding-vpptokenstate.md)
- [<span data-ttu-id="b78fa-142">Status de sincronização do token VPP</span><span class="sxs-lookup"><span data-stu-id="b78fa-142">VPP token sync status</span></span>](intune-onboarding-vpptokensyncstatus.md)
- [<span data-ttu-id="b78fa-143">Uso do PIN do Windows Hello para empresas</span><span class="sxs-lookup"><span data-stu-id="b78fa-143">Windows Hello for business PIN usage</span></span>](intune-onboarding-windowshelloforbusinesspinusage.md)