---
title: Registrar dispositivos corporativos usando o Intune - API do Microsoft Graph
description: Lista a API do Microsoft Graph para pontos de extremidade do Intune (REST) que registram dispositivos para uma organização de locatários.
author: dougeby
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a85db8c4397659789feafa395195a39542928f01
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131950"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a><span data-ttu-id="73bc4-103">Registrar dispositivos de propriedade corporativa por meio do Intune</span><span class="sxs-lookup"><span data-stu-id="73bc4-103">Enroll corporate-owned devices by using Intune</span></span>

<span data-ttu-id="73bc4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73bc4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="73bc4-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="73bc4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73bc4-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="73bc4-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="73bc4-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="73bc4-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73bc4-108">É possível registrar dispositivos pertencentes à organização ou de propriedade corporativa para serem gerenciados com o Intune de várias maneiras, dependendo do tipo de dispositivo, de como o dispositivo foi comprado e das necessidades da organização.</span><span class="sxs-lookup"><span data-stu-id="73bc4-108">You can enroll organization-owned or corporate-owned devices to manage with Intune in a variety of ways, depending on the type of device, how the device was purchased, and the needs of the organization.</span></span> <span data-ttu-id="73bc4-109">Também é possível instalar o aplicativo Portal da Empresa para registrar e gerenciar dispositivos de propriedade corporativa, como em um cenário "traga seu próprio dispositivo" (BYOD).</span><span class="sxs-lookup"><span data-stu-id="73bc4-109">You also can install the Company Portal app to enroll and manage corporate-owned devices, like in a "bring your own device" (BYOD) scenario.</span></span>

<span data-ttu-id="73bc4-110">Os seguintes recursos do Graph estão disponíveis para gerenciar dispositivos corporativos no Intune:</span><span class="sxs-lookup"><span data-stu-id="73bc4-110">The following Graph resources are available to manage corporate-owned devices in Intune:</span></span>

- [<span data-ttu-id="73bc4-111">Perfil de implantação do Windows Autopilot do Active Directory</span><span class="sxs-lookup"><span data-stu-id="73bc4-111">Active directory windows autopilot deployment profile</span></span>](intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="73bc4-112">Atribuição de perfil de registro da Apple</span><span class="sxs-lookup"><span data-stu-id="73bc4-112">Apple enrollment profile assignment</span></span>](intune-enrollment-appleenrollmentprofileassignment.md)
- [<span data-ttu-id="73bc4-113">Tipo de registro de tipo de proprietário da Apple</span><span class="sxs-lookup"><span data-stu-id="73bc4-113">Apple owner type enrollment type</span></span>](intune-enrollment-appleownertypeenrollmenttype.md)
- [<span data-ttu-id="73bc4-114">Perfil de registro iniciado pelo usuário apple</span><span class="sxs-lookup"><span data-stu-id="73bc4-114">Apple user initiated enrollment profile</span></span>](intune-enrollment-appleuserinitiatedenrollmentprofile.md)
- [<span data-ttu-id="73bc4-115">Tipo de registro iniciado pelo usuário apple</span><span class="sxs-lookup"><span data-stu-id="73bc4-115">Apple user initiated enrollment type</span></span>](intune-enrollment-appleuserinitiatedenrollmenttype.md)
- [<span data-ttu-id="73bc4-116">Perfil de implantação do Windows Autopilot do Azure AD</span><span class="sxs-lookup"><span data-stu-id="73bc4-116">Azure AD windows autopilot deployment profile</span></span>](intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="73bc4-117">Estado do dispositivo windows autopilot excluído</span><span class="sxs-lookup"><span data-stu-id="73bc4-117">Deleted windows autopilot device state</span></span>](intune-enrollment-deletedwindowsautopilotdevicestate.md)
- [<span data-ttu-id="73bc4-118">Perfil básico de registro do DEP</span><span class="sxs-lookup"><span data-stu-id="73bc4-118">DEP enrollment base profile</span></span>](intune-enrollment-depenrollmentbaseprofile.md)
- [<span data-ttu-id="73bc4-119">Perfil de registro do DEP</span><span class="sxs-lookup"><span data-stu-id="73bc4-119">DEP enrollment profile</span></span>](intune-enrollment-depenrollmentprofile.md)
- [<span data-ttu-id="73bc4-120">Perfil de registro de iOS do DEP</span><span class="sxs-lookup"><span data-stu-id="73bc4-120">DEP iOS enrollment profile</span></span>](intune-enrollment-depiosenrollmentprofile.md)
- [<span data-ttu-id="73bc4-121">Perfil de registro de macOS do DEP</span><span class="sxs-lookup"><span data-stu-id="73bc4-121">DEP macOS enrollment profile</span></span>](intune-enrollment-depmacosenrollmentprofile.md)
- [<span data-ttu-id="73bc4-122">Configuração de integração do DEP</span><span class="sxs-lookup"><span data-stu-id="73bc4-122">DEP on-boarding setting</span></span>](intune-enrollment-deponboardingsetting.md)
- [<span data-ttu-id="73bc4-123">Tipo de token do DEP</span><span class="sxs-lookup"><span data-stu-id="73bc4-123">DEP token type</span></span>](intune-enrollment-deptokentype.md)
- [<span data-ttu-id="73bc4-124">Fonte de descoberta</span><span class="sxs-lookup"><span data-stu-id="73bc4-124">Discovery source</span></span>](intune-enrollment-discoverysource.md)
- [<span data-ttu-id="73bc4-125">Perfil de registro</span><span class="sxs-lookup"><span data-stu-id="73bc4-125">Enrollment profile</span></span>](intune-enrollment-enrollmentprofile.md)
- [<span data-ttu-id="73bc4-126">Identidade do dispositivo Apple importada</span><span class="sxs-lookup"><span data-stu-id="73bc4-126">Imported Apple device identity</span></span>](intune-enrollment-importedappledeviceidentity.md)
- [<span data-ttu-id="73bc4-127">Importar resultado de identidade do dispositivo Apple</span><span class="sxs-lookup"><span data-stu-id="73bc4-127">Imported Apple device identity result</span></span>](intune-enrollment-importedappledeviceidentityresult.md)
- [<span data-ttu-id="73bc4-128">Identidade do dispositivo importada</span><span class="sxs-lookup"><span data-stu-id="73bc4-128">Imported device identity</span></span>](intune-enrollment-importeddeviceidentity.md)
- [<span data-ttu-id="73bc4-129">Resultado de identidade do dispositivo importada</span><span class="sxs-lookup"><span data-stu-id="73bc4-129">Imported device identity result</span></span>](intune-enrollment-importeddeviceidentityresult.md)
- [<span data-ttu-id="73bc4-130">Tipo de identidade do dispositivo importada</span><span class="sxs-lookup"><span data-stu-id="73bc4-130">Imported device identity type</span></span>](intune-enrollment-importeddeviceidentitytype.md)
- [<span data-ttu-id="73bc4-131">Identidade importada do dispositivo do Windows autopilot</span><span class="sxs-lookup"><span data-stu-id="73bc4-131">Imported windows autopilot device identity</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [<span data-ttu-id="73bc4-132">Status de importação da identidade de dispositivo importada do windows autopilot</span><span class="sxs-lookup"><span data-stu-id="73bc4-132">Imported windows autopilot device identity import status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [<span data-ttu-id="73bc4-133">Estado de identidade de dispositivo importado do windows autopilot</span><span class="sxs-lookup"><span data-stu-id="73bc4-133">Imported windows autopilot device identity state</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [<span data-ttu-id="73bc4-134">Status de carregamento da identidade de dispositivo importado do windows autopilot</span><span class="sxs-lookup"><span data-stu-id="73bc4-134">Imported windows autopilot device identity upload status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [<span data-ttu-id="73bc4-135">Modo de emparelhamento do iTunes</span><span class="sxs-lookup"><span data-stu-id="73bc4-135">iTunes pairing mode</span></span>](intune-enrollment-itunespairingmode.md)
- [<span data-ttu-id="73bc4-136">Certificado de gerenciamento com impressão digital</span><span class="sxs-lookup"><span data-stu-id="73bc4-136">Management certificate with thumbprint</span></span>](intune-enrollment-managementcertificatewiththumbprint.md)
- [<span data-ttu-id="73bc4-137">Configurações de experiência iniciais</span><span class="sxs-lookup"><span data-stu-id="73bc4-137">Out of box experience settings</span></span>](intune-enrollment-outofboxexperiencesettings.md)
- [<span data-ttu-id="73bc4-138">Plataforma</span><span class="sxs-lookup"><span data-stu-id="73bc4-138">Platform</span></span>](intune-enrollment-platform.md)
- [<span data-ttu-id="73bc4-139">Limite de inscrição sugerido</span><span class="sxs-lookup"><span data-stu-id="73bc4-139">Suggested enrollment limit</span></span>](intune-enrollment-suggestedenrollmentlimit.md)
- [<span data-ttu-id="73bc4-140">Atribuição do perfil de implantação do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="73bc4-140">Windows autopilot deployment profile assignment</span></span>](intune-enrollment-windowsautopilotdeploymentprofileassignment.md)
- [<span data-ttu-id="73bc4-141">Estado de exclusão de dispositivo do Windows autopilot</span><span class="sxs-lookup"><span data-stu-id="73bc4-141">Windows autopilot device deletion state</span></span>](intune-enrollment-windowsautopilotdevicedeletionstate.md)
- [<span data-ttu-id="73bc4-142">Identidade do dispositivo do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="73bc4-142">Windows autopilot device identity</span></span>](intune-enrollment-windowsautopilotdeviceidentity.md)
- [<span data-ttu-id="73bc4-143">Tipo de dispositivo do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="73bc4-143">Windows autopilot device type</span></span>](intune-enrollment-windowsautopilotdevicetype.md)
- [<span data-ttu-id="73bc4-144">Status detalhado de atribuição do perfil do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="73bc4-144">Windows autopilot profile assignment detailed status</span></span>](intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)
- [<span data-ttu-id="73bc4-145">Status de atribuição do perfil do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="73bc4-145">Windows autopilot profile assignment status</span></span>](intune-enrollment-windowsautopilotprofileassignmentstatus.md)
- [<span data-ttu-id="73bc4-146">Configurações do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="73bc4-146">Windows autopilot settings</span></span>](intune-enrollment-windowsautopilotsettings.md)
- [<span data-ttu-id="73bc4-147">Status de sincronização do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="73bc4-147">Windows autopilot sync status</span></span>](intune-enrollment-windowsautopilotsyncstatus.md)
- [<span data-ttu-id="73bc4-148">Tipo de uso do dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="73bc4-148">Windows device usage type</span></span>](intune-enrollment-windowsdeviceusagetype.md)
- [<span data-ttu-id="73bc4-149">Configurações de tela de status de registro do Windows</span><span class="sxs-lookup"><span data-stu-id="73bc4-149">Windows enrollment status screen settings</span></span>](intune-enrollment-windowsenrollmentstatusscreensettings.md)
- [<span data-ttu-id="73bc4-150">Tipo de usuário do Windows</span><span class="sxs-lookup"><span data-stu-id="73bc4-150">Windows user type</span></span>](intune-enrollment-windowsusertype.md)