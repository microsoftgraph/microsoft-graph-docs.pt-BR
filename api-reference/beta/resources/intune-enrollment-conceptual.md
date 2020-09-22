---
title: Registrar dispositivos corporativos usando o Intune-Microsoft Graph API
description: Lista a API do Microsoft Graph para os pontos de extremidade do Intune (REST) que registram dispositivos para uma organização de locatário.
author: dougeby
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 250303d1aad682e3f77dfbdfdccb335802e72b51
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080352"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a><span data-ttu-id="c419f-103">Registrar dispositivos de propriedade corporativa por meio do Intune</span><span class="sxs-lookup"><span data-stu-id="c419f-103">Enroll corporate-owned devices by using Intune</span></span>

<span data-ttu-id="c419f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c419f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c419f-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c419f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c419f-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c419f-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c419f-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c419f-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c419f-108">É possível registrar dispositivos pertencentes à organização ou de propriedade corporativa para serem gerenciados com o Intune de várias maneiras, dependendo do tipo de dispositivo, de como o dispositivo foi comprado e das necessidades da organização.</span><span class="sxs-lookup"><span data-stu-id="c419f-108">You can enroll organization-owned or corporate-owned devices to manage with Intune in a variety of ways, depending on the type of device, how the device was purchased, and the needs of the organization.</span></span> <span data-ttu-id="c419f-109">Também é possível instalar o aplicativo Portal da Empresa para registrar e gerenciar dispositivos de propriedade corporativa, como em um cenário "traga seu próprio dispositivo" (BYOD).</span><span class="sxs-lookup"><span data-stu-id="c419f-109">You also can install the Company Portal app to enroll and manage corporate-owned devices, like in a "bring your own device" (BYOD) scenario.</span></span>

<span data-ttu-id="c419f-110">Os seguintes recursos do Graph estão disponíveis para gerenciar dispositivos corporativos no Intune:</span><span class="sxs-lookup"><span data-stu-id="c419f-110">The following Graph resources are available to manage corporate-owned devices in Intune:</span></span>

- [<span data-ttu-id="c419f-111">Perfil de implantação do Windows Autopilot do Active Directory</span><span class="sxs-lookup"><span data-stu-id="c419f-111">Active directory windows autopilot deployment profile</span></span>](intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="c419f-112">Atribuição de perfil de registro da Apple</span><span class="sxs-lookup"><span data-stu-id="c419f-112">Apple enrollment profile assignment</span></span>](intune-enrollment-appleenrollmentprofileassignment.md)
- [<span data-ttu-id="c419f-113">Tipo de registro de tipo de proprietário da Apple</span><span class="sxs-lookup"><span data-stu-id="c419f-113">Apple owner type enrollment type</span></span>](intune-enrollment-appleownertypeenrollmenttype.md)
- [<span data-ttu-id="c419f-114">Perfil de registro iniciado pelo usuário da Apple</span><span class="sxs-lookup"><span data-stu-id="c419f-114">Apple user initiated enrollment profile</span></span>](intune-enrollment-appleuserinitiatedenrollmentprofile.md)
- [<span data-ttu-id="c419f-115">Tipo de registro iniciado pelo usuário da Apple</span><span class="sxs-lookup"><span data-stu-id="c419f-115">Apple user initiated enrollment type</span></span>](intune-enrollment-appleuserinitiatedenrollmenttype.md)
- [<span data-ttu-id="c419f-116">Perfil de implantação do Windows Autopilot do Azure AD</span><span class="sxs-lookup"><span data-stu-id="c419f-116">Azure AD windows autopilot deployment profile</span></span>](intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="c419f-117">Perfil básico de registro do DEP</span><span class="sxs-lookup"><span data-stu-id="c419f-117">DEP enrollment base profile</span></span>](intune-enrollment-depenrollmentbaseprofile.md)
- [<span data-ttu-id="c419f-118">Perfil de registro do DEP</span><span class="sxs-lookup"><span data-stu-id="c419f-118">DEP enrollment profile</span></span>](intune-enrollment-depenrollmentprofile.md)
- [<span data-ttu-id="c419f-119">Perfil de registro de iOS do DEP</span><span class="sxs-lookup"><span data-stu-id="c419f-119">DEP iOS enrollment profile</span></span>](intune-enrollment-depiosenrollmentprofile.md)
- [<span data-ttu-id="c419f-120">Perfil de registro de macOS do DEP</span><span class="sxs-lookup"><span data-stu-id="c419f-120">DEP macOS enrollment profile</span></span>](intune-enrollment-depmacosenrollmentprofile.md)
- [<span data-ttu-id="c419f-121">Configuração de integração do DEP</span><span class="sxs-lookup"><span data-stu-id="c419f-121">DEP on-boarding setting</span></span>](intune-enrollment-deponboardingsetting.md)
- [<span data-ttu-id="c419f-122">Tipo de token do DEP</span><span class="sxs-lookup"><span data-stu-id="c419f-122">DEP token type</span></span>](intune-enrollment-deptokentype.md)
- [<span data-ttu-id="c419f-123">Fonte de descoberta</span><span class="sxs-lookup"><span data-stu-id="c419f-123">Discovery source</span></span>](intune-enrollment-discoverysource.md)
- [<span data-ttu-id="c419f-124">Perfil de registro</span><span class="sxs-lookup"><span data-stu-id="c419f-124">Enrollment profile</span></span>](intune-enrollment-enrollmentprofile.md)
- [<span data-ttu-id="c419f-125">Identidade do dispositivo Apple importada</span><span class="sxs-lookup"><span data-stu-id="c419f-125">Imported Apple device identity</span></span>](intune-enrollment-importedappledeviceidentity.md)
- [<span data-ttu-id="c419f-126">Importar resultado de identidade do dispositivo Apple</span><span class="sxs-lookup"><span data-stu-id="c419f-126">Imported Apple device identity result</span></span>](intune-enrollment-importedappledeviceidentityresult.md)
- [<span data-ttu-id="c419f-127">Identidade do dispositivo importada</span><span class="sxs-lookup"><span data-stu-id="c419f-127">Imported device identity</span></span>](intune-enrollment-importeddeviceidentity.md)
- [<span data-ttu-id="c419f-128">Resultado de identidade do dispositivo importada</span><span class="sxs-lookup"><span data-stu-id="c419f-128">Imported device identity result</span></span>](intune-enrollment-importeddeviceidentityresult.md)
- [<span data-ttu-id="c419f-129">Tipo de identidade do dispositivo importada</span><span class="sxs-lookup"><span data-stu-id="c419f-129">Imported device identity type</span></span>](intune-enrollment-importeddeviceidentitytype.md)
- [<span data-ttu-id="c419f-130">Identidade importada do dispositivo do Windows autopilot</span><span class="sxs-lookup"><span data-stu-id="c419f-130">Imported windows autopilot device identity</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [<span data-ttu-id="c419f-131">Status de importação da identidade de dispositivo importada do windows autopilot</span><span class="sxs-lookup"><span data-stu-id="c419f-131">Imported windows autopilot device identity import status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [<span data-ttu-id="c419f-132">Estado de identidade de dispositivo importado do windows autopilot</span><span class="sxs-lookup"><span data-stu-id="c419f-132">Imported windows autopilot device identity state</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [<span data-ttu-id="c419f-133">Status de carregamento da identidade de dispositivo importado do windows autopilot</span><span class="sxs-lookup"><span data-stu-id="c419f-133">Imported windows autopilot device identity upload status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [<span data-ttu-id="c419f-134">Modo de emparelhamento do iTunes</span><span class="sxs-lookup"><span data-stu-id="c419f-134">iTunes pairing mode</span></span>](intune-enrollment-itunespairingmode.md)
- [<span data-ttu-id="c419f-135">Certificado de gerenciamento com impressão digital</span><span class="sxs-lookup"><span data-stu-id="c419f-135">Management certificate with thumbprint</span></span>](intune-enrollment-managementcertificatewiththumbprint.md)
- [<span data-ttu-id="c419f-136">Configurações de experiência iniciais</span><span class="sxs-lookup"><span data-stu-id="c419f-136">Out of box experience settings</span></span>](intune-enrollment-outofboxexperiencesettings.md)
- [<span data-ttu-id="c419f-137">Plataforma</span><span class="sxs-lookup"><span data-stu-id="c419f-137">Platform</span></span>](intune-enrollment-platform.md)
- [<span data-ttu-id="c419f-138">Limite de registro sugerido</span><span class="sxs-lookup"><span data-stu-id="c419f-138">Suggested enrollment limit</span></span>](intune-enrollment-suggestedenrollmentlimit.md)
- [<span data-ttu-id="c419f-139">Atribuição do perfil de implantação do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="c419f-139">Windows autopilot deployment profile assignment</span></span>](intune-enrollment-windowsautopilotdeploymentprofileassignment.md)
- [<span data-ttu-id="c419f-140">Identidade do dispositivo do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="c419f-140">Windows autopilot device identity</span></span>](intune-enrollment-windowsautopilotdeviceidentity.md)
- [<span data-ttu-id="c419f-141">Tipo de dispositivo do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="c419f-141">Windows autopilot device type</span></span>](intune-enrollment-windowsautopilotdevicetype.md)
- [<span data-ttu-id="c419f-142">Status detalhado de atribuição do perfil do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="c419f-142">Windows autopilot profile assignment detailed status</span></span>](intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)
- [<span data-ttu-id="c419f-143">Status de atribuição do perfil do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="c419f-143">Windows autopilot profile assignment status</span></span>](intune-enrollment-windowsautopilotprofileassignmentstatus.md)
- [<span data-ttu-id="c419f-144">Configurações do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="c419f-144">Windows autopilot settings</span></span>](intune-enrollment-windowsautopilotsettings.md)
- [<span data-ttu-id="c419f-145">Status de sincronização do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="c419f-145">Windows autopilot sync status</span></span>](intune-enrollment-windowsautopilotsyncstatus.md)
- [<span data-ttu-id="c419f-146">Tipo de uso do dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="c419f-146">Windows device usage type</span></span>](intune-enrollment-windowsdeviceusagetype.md)
- [<span data-ttu-id="c419f-147">Configurações de tela de status de registro do Windows</span><span class="sxs-lookup"><span data-stu-id="c419f-147">Windows enrollment status screen settings</span></span>](intune-enrollment-windowsenrollmentstatusscreensettings.md)
- [<span data-ttu-id="c419f-148">Tipo de usuário do Windows</span><span class="sxs-lookup"><span data-stu-id="c419f-148">Windows user type</span></span>](intune-enrollment-windowsusertype.md)


