---
title: Registrar dispositivos corporativos usando o Intune-Microsoft Graph API
description: Lista a API do Microsoft Graph para os pontos de extremidade do Intune (REST) que registram dispositivos para uma organização de locatário.
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5655bd1733c2383bac562f700be5abc1c57bf43b
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196606"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a><span data-ttu-id="460e2-103">Registrar dispositivos de propriedade corporativa por meio do Intune</span><span class="sxs-lookup"><span data-stu-id="460e2-103">Enroll corporate-owned devices by using Intune</span></span>

> <span data-ttu-id="460e2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="460e2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="460e2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="460e2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="460e2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="460e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="460e2-107">É possível registrar dispositivos pertencentes à organização ou de propriedade corporativa para serem gerenciados com o Intune de várias maneiras, dependendo do tipo de dispositivo, de como o dispositivo foi comprado e das necessidades da organização.</span><span class="sxs-lookup"><span data-stu-id="460e2-107">You can enroll organization-owned or corporate-owned devices to manage with Intune in a variety of ways, depending on the type of device, how the device was purchased, and the needs of the organization.</span></span> <span data-ttu-id="460e2-108">Também é possível instalar o aplicativo Portal da Empresa para registrar e gerenciar dispositivos de propriedade corporativa, como em um cenário "traga seu próprio dispositivo" (BYOD).</span><span class="sxs-lookup"><span data-stu-id="460e2-108">You also can install the Company Portal app to enroll and manage corporate-owned devices, like in a "bring your own device" (BYOD) scenario.</span></span>

<span data-ttu-id="460e2-109">Os seguintes recursos do Graph estão disponíveis para gerenciar dispositivos corporativos no Intune:</span><span class="sxs-lookup"><span data-stu-id="460e2-109">The following Graph resources are available to manage corporate-owned devices in Intune:</span></span>

- [<span data-ttu-id="460e2-110">Perfil de implantação do Windows Autopilot do Active Directory</span><span class="sxs-lookup"><span data-stu-id="460e2-110">Active directory windows autopilot deployment profile</span></span>](intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="460e2-111">Atribuição de perfil de registro da Apple</span><span class="sxs-lookup"><span data-stu-id="460e2-111">Apple enrollment profile assignment</span></span>](intune-enrollment-appleenrollmentprofileassignment.md)
- [<span data-ttu-id="460e2-112">Tipo de registro de tipo de proprietário da Apple</span><span class="sxs-lookup"><span data-stu-id="460e2-112">Apple owner type enrollment type</span></span>](intune-enrollment-appleownertypeenrollmenttype.md)
- [<span data-ttu-id="460e2-113">Perfil de registro iniciado pelo usuário da Apple</span><span class="sxs-lookup"><span data-stu-id="460e2-113">Apple user initiated enrollment profile</span></span>](intune-enrollment-appleuserinitiatedenrollmentprofile.md)
- [<span data-ttu-id="460e2-114">Tipo de registro iniciado pelo usuário da Apple</span><span class="sxs-lookup"><span data-stu-id="460e2-114">Apple user initiated enrollment type</span></span>](intune-enrollment-appleuserinitiatedenrollmenttype.md)
- [<span data-ttu-id="460e2-115">Perfil de implantação do Windows Autopilot do Azure AD</span><span class="sxs-lookup"><span data-stu-id="460e2-115">Azure AD windows autopilot deployment profile</span></span>](intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="460e2-116">Perfil básico de registro do DEP</span><span class="sxs-lookup"><span data-stu-id="460e2-116">DEP enrollment base profile</span></span>](intune-enrollment-depenrollmentbaseprofile.md)
- [<span data-ttu-id="460e2-117">Perfil de registro do DEP</span><span class="sxs-lookup"><span data-stu-id="460e2-117">DEP enrollment profile</span></span>](intune-enrollment-depenrollmentprofile.md)
- [<span data-ttu-id="460e2-118">Perfil de registro de iOS do DEP</span><span class="sxs-lookup"><span data-stu-id="460e2-118">DEP iOS enrollment profile</span></span>](intune-enrollment-depiosenrollmentprofile.md)
- [<span data-ttu-id="460e2-119">Perfil de registro de macOS do DEP</span><span class="sxs-lookup"><span data-stu-id="460e2-119">DEP macOS enrollment profile</span></span>](intune-enrollment-depmacosenrollmentprofile.md)
- [<span data-ttu-id="460e2-120">Configuração de integração do DEP</span><span class="sxs-lookup"><span data-stu-id="460e2-120">DEP on-boarding setting</span></span>](intune-enrollment-deponboardingsetting.md)
- [<span data-ttu-id="460e2-121">Tipo de token do DEP</span><span class="sxs-lookup"><span data-stu-id="460e2-121">DEP token type</span></span>](intune-enrollment-deptokentype.md)
- [<span data-ttu-id="460e2-122">Fonte de descoberta</span><span class="sxs-lookup"><span data-stu-id="460e2-122">Discovery source</span></span>](intune-enrollment-discoverysource.md)
- [<span data-ttu-id="460e2-123">Perfil de registro</span><span class="sxs-lookup"><span data-stu-id="460e2-123">Enrollment profile</span></span>](intune-enrollment-enrollmentprofile.md)
- [<span data-ttu-id="460e2-124">Identidade do dispositivo Apple importada</span><span class="sxs-lookup"><span data-stu-id="460e2-124">Imported Apple device identity</span></span>](intune-enrollment-importedappledeviceidentity.md)
- [<span data-ttu-id="460e2-125">Importar resultado de identidade do dispositivo Apple</span><span class="sxs-lookup"><span data-stu-id="460e2-125">Imported Apple device identity result</span></span>](intune-enrollment-importedappledeviceidentityresult.md)
- [<span data-ttu-id="460e2-126">Identidade do dispositivo importada</span><span class="sxs-lookup"><span data-stu-id="460e2-126">Imported device identity</span></span>](intune-enrollment-importeddeviceidentity.md)
- [<span data-ttu-id="460e2-127">Resultado de identidade do dispositivo importada</span><span class="sxs-lookup"><span data-stu-id="460e2-127">Imported device identity result</span></span>](intune-enrollment-importeddeviceidentityresult.md)
- [<span data-ttu-id="460e2-128">Tipo de identidade do dispositivo importada</span><span class="sxs-lookup"><span data-stu-id="460e2-128">Imported device identity type</span></span>](intune-enrollment-importeddeviceidentitytype.md)
- [<span data-ttu-id="460e2-129">Identidade importada do dispositivo do Windows autopilot</span><span class="sxs-lookup"><span data-stu-id="460e2-129">Imported windows autopilot device identity</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [<span data-ttu-id="460e2-130">Status de importação da identidade de dispositivo importada do windows autopilot</span><span class="sxs-lookup"><span data-stu-id="460e2-130">Imported windows autopilot device identity import status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [<span data-ttu-id="460e2-131">Estado de identidade de dispositivo importado do windows autopilot</span><span class="sxs-lookup"><span data-stu-id="460e2-131">Imported windows autopilot device identity state</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [<span data-ttu-id="460e2-132">Status de carregamento da identidade de dispositivo importado do windows autopilot</span><span class="sxs-lookup"><span data-stu-id="460e2-132">Imported windows autopilot device identity upload status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [<span data-ttu-id="460e2-133">Modo de emparelhamento do iTunes</span><span class="sxs-lookup"><span data-stu-id="460e2-133">iTunes pairing mode</span></span>](intune-enrollment-itunespairingmode.md)
- [<span data-ttu-id="460e2-134">Certificado de gerenciamento com impressão digital</span><span class="sxs-lookup"><span data-stu-id="460e2-134">Management certificate with thumbprint</span></span>](intune-enrollment-managementcertificatewiththumbprint.md)
- [<span data-ttu-id="460e2-135">Configurações de experiência iniciais</span><span class="sxs-lookup"><span data-stu-id="460e2-135">Out of box experience settings</span></span>](intune-enrollment-outofboxexperiencesettings.md)
- [<span data-ttu-id="460e2-136">Plataforma</span><span class="sxs-lookup"><span data-stu-id="460e2-136">Platform</span></span>](intune-enrollment-platform.md)
- [<span data-ttu-id="460e2-137">Atribuição do perfil de implantação do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="460e2-137">Windows autopilot deployment profile assignment</span></span>](intune-enrollment-windowsautopilotdeploymentprofileassignment.md)
- [<span data-ttu-id="460e2-138">Identidade do dispositivo do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="460e2-138">Windows autopilot device identity</span></span>](intune-enrollment-windowsautopilotdeviceidentity.md)
- [<span data-ttu-id="460e2-139">Tipo de dispositivo do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="460e2-139">Windows autopilot device type</span></span>](intune-enrollment-windowsautopilotdevicetype.md)
- [<span data-ttu-id="460e2-140">Status detalhado de atribuição do perfil do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="460e2-140">Windows autopilot profile assignment detailed status</span></span>](intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)
- [<span data-ttu-id="460e2-141">Status de atribuição do perfil do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="460e2-141">Windows autopilot profile assignment status</span></span>](intune-enrollment-windowsautopilotprofileassignmentstatus.md)
- [<span data-ttu-id="460e2-142">Configurações do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="460e2-142">Windows autopilot settings</span></span>](intune-enrollment-windowsautopilotsettings.md)
- [<span data-ttu-id="460e2-143">Status de sincronização do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="460e2-143">Windows autopilot sync status</span></span>](intune-enrollment-windowsautopilotsyncstatus.md)
- [<span data-ttu-id="460e2-144">Tipo de uso do dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="460e2-144">Windows device usage type</span></span>](intune-enrollment-windowsdeviceusagetype.md)
- [<span data-ttu-id="460e2-145">Configurações de tela de status de registro do Windows</span><span class="sxs-lookup"><span data-stu-id="460e2-145">Windows enrollment status screen settings</span></span>](intune-enrollment-windowsenrollmentstatusscreensettings.md)
- [<span data-ttu-id="460e2-146">Tipo de usuário do Windows</span><span class="sxs-lookup"><span data-stu-id="460e2-146">Windows user type</span></span>](intune-enrollment-windowsusertype.md)

