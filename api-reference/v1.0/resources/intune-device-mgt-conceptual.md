---
title: Gerenciamento de dispositivos no Microsoft Intune
description: ''
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4c8f6676647405e8186e9d27466266f6690e2cd1
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250065"
---
# <a name="device-management-in-microsoft-intune"></a><span data-ttu-id="152d4-102">Gerenciamento de dispositivos no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="152d4-102">Device management in Microsoft Intune</span></span>

> <span data-ttu-id="152d4-103">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="152d4-103">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

- [<span data-ttu-id="152d4-104">Estado da ação</span><span class="sxs-lookup"><span data-stu-id="152d4-104">Action state</span></span>](intune-devices-actionstate.md)
- [<span data-ttu-id="152d4-105">Certificado de notificação por push da Apple</span><span class="sxs-lookup"><span data-stu-id="152d4-105">Apple push notification certificate</span></span>](intune-devices-applepushnotificationcertificate.md)
- [<span data-ttu-id="152d4-106">Ator de auditoria</span><span class="sxs-lookup"><span data-stu-id="152d4-106">Audit actor</span></span>](intune-auditing-auditactor.md)
- [<span data-ttu-id="152d4-107">Evento de auditoria</span><span class="sxs-lookup"><span data-stu-id="152d4-107">Audit event</span></span>](intune-auditing-auditevent.md)
- [<span data-ttu-id="152d4-108">Propriedade de auditoria</span><span class="sxs-lookup"><span data-stu-id="152d4-108">Audit property</span></span>](intune-auditing-auditproperty.md)
- [<span data-ttu-id="152d4-109">Recurso de auditoria</span><span class="sxs-lookup"><span data-stu-id="152d4-109">Audit resource</span></span>](intune-auditing-auditresource.md)
- [<span data-ttu-id="152d4-110">Estado de conformidade</span><span class="sxs-lookup"><span data-stu-id="152d4-110">Compliance state</span></span>](intune-devices-compliancestate.md)
- [<span data-ttu-id="152d4-111">Recursos habilitados pelo cliente do Gerenciador de Configurações</span><span class="sxs-lookup"><span data-stu-id="152d4-111">Configuration manager client enabled features</span></span>](intune-devices-configurationmanagerclientenabledfeatures.md)
- [<span data-ttu-id="152d4-112">Resultado da ação de excluir o usuário do dispositivo compartilhado da Apple</span><span class="sxs-lookup"><span data-stu-id="152d4-112">Delete user from shared Apple device action result</span></span>](intune-devices-deleteuserfromsharedappledeviceactionresult.md)
- [<span data-ttu-id="152d4-113">Aplicativo detectado</span><span class="sxs-lookup"><span data-stu-id="152d4-113">Detected app</span></span>](intune-devices-detectedapp.md)
- [<span data-ttu-id="152d4-114">Resultado da ação do dispositivo</span><span class="sxs-lookup"><span data-stu-id="152d4-114">Device action result</span></span>](intune-devices-deviceactionresult.md)
- [<span data-ttu-id="152d4-115">Motivo da falha de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="152d4-115">Device enrollment failure reason</span></span>](intune-troubleshooting-deviceenrollmentfailurereason.md)
- [<span data-ttu-id="152d4-116">Resumo do Estado de Acesso ao Exchange do dispositivo</span><span class="sxs-lookup"><span data-stu-id="152d4-116">Device exchange access state summary</span></span>](intune-devices-deviceexchangeaccessstatesummary.md)
- [<span data-ttu-id="152d4-117">Geolocalização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="152d4-117">Device geolocation</span></span>](intune-devices-devicegeolocation.md)
- [<span data-ttu-id="152d4-118">Estado do atestado de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="152d4-118">Device health attestation state</span></span>](intune-devices-devicehealthattestationstate.md)
- [<span data-ttu-id="152d4-119">Estado de acesso do Exchange de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="152d4-119">Device management exchange access state</span></span>](intune-devices-devicemanagementexchangeaccessstate.md)
- [<span data-ttu-id="152d4-120">Motivo do estado de acesso do Exchange de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="152d4-120">Device management exchange access state reason</span></span>](intune-devices-devicemanagementexchangeaccessstatereason.md)
- [<span data-ttu-id="152d4-121">Estado de assinatura de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="152d4-121">Device management subscription state</span></span>](intune-devices-devicemanagementsubscriptionstate.md)
- [<span data-ttu-id="152d4-122">Evento de solução de problemas com o gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="152d4-122">Device management troubleshooting event</span></span>](intune-troubleshooting-devicemanagementtroubleshootingevent.md)
- [<span data-ttu-id="152d4-123">Resumo do sistema operacional do dispositivo</span><span class="sxs-lookup"><span data-stu-id="152d4-123">Device operating system summary</span></span>](intune-devices-deviceoperatingsystemsummary.md)
- [<span data-ttu-id="152d4-124">Estado do registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="152d4-124">Device registration state</span></span>](intune-devices-deviceregistrationstate.md)
- [<span data-ttu-id="152d4-125">Evento de solução de problemas de registro</span><span class="sxs-lookup"><span data-stu-id="152d4-125">Enrollment troubleshooting event</span></span>](intune-troubleshooting-enrollmenttroubleshootingevent.md)
- [<span data-ttu-id="152d4-126">Mensagem de notificação localizada</span><span class="sxs-lookup"><span data-stu-id="152d4-126">Localized notification message</span></span>](intune-notification-localizednotificationmessage.md)
- [<span data-ttu-id="152d4-127">Resultado da ação de localizar dispositivo</span><span class="sxs-lookup"><span data-stu-id="152d4-127">Locate device action result</span></span>](intune-devices-locatedeviceactionresult.md)
- [<span data-ttu-id="152d4-128">Dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="152d4-128">Managed device</span></span>](intune-devices-manageddevice.md)
- [<span data-ttu-id="152d4-129">Visão geral do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="152d4-129">Managed device overview</span></span>](intune-devices-manageddeviceoverview.md)
- [<span data-ttu-id="152d4-130">Tipo de proprietário do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="152d4-130">Managed device owner type</span></span>](intune-devices-manageddeviceownertype.md)
- [<span data-ttu-id="152d4-131">Estado de integridade reportado pelo parceiro do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="152d4-131">Managed device partner reported health state</span></span>](intune-devices-manageddevicepartnerreportedhealthstate.md)
- [<span data-ttu-id="152d4-132">Tipo de agente de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="152d4-132">Management agent type</span></span>](intune-devices-managementagenttype.md)
- [<span data-ttu-id="152d4-133">Modelo de mensagem de notificação</span><span class="sxs-lookup"><span data-stu-id="152d4-133">Notification message template</span></span>](intune-notification-notificationmessagetemplate.md)
- [<span data-ttu-id="152d4-134">Opções de identidade visual do modelo de notificação</span><span class="sxs-lookup"><span data-stu-id="152d4-134">Notification template branding options</span></span>](intune-notification-notificationtemplatebrandingoptions.md)
- [<span data-ttu-id="152d4-135">Status da inclusão de assistência remota</span><span class="sxs-lookup"><span data-stu-id="152d4-135">Remote assistance on-boarding status</span></span>](intune-remoteassistance-remoteassistanceonboardingstatus.md)
- [<span data-ttu-id="152d4-136">Parceiro de assistência remota</span><span class="sxs-lookup"><span data-stu-id="152d4-136">Remote assistance partner</span></span>](intune-remoteassistance-remoteassistancepartner.md)
- [<span data-ttu-id="152d4-137">Resultado da ação de bloqueio remoto</span><span class="sxs-lookup"><span data-stu-id="152d4-137">Remote lock action result</span></span>](intune-devices-remotelockactionresult.md)
- [<span data-ttu-id="152d4-138">Resultado da ação de redefinir a senha</span><span class="sxs-lookup"><span data-stu-id="152d4-138">Reset passcode action result</span></span>](intune-devices-resetpasscodeactionresult.md)
- [<span data-ttu-id="152d4-139">Parâmetro da ação de atualização de conta de dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="152d4-139">Update windows device account action parameter</span></span>](intune-devices-updatewindowsdeviceaccountactionparameter.md)
- [<span data-ttu-id="152d4-140">Resultado da ação de verificação do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="152d4-140">Windows defender scan action result</span></span>](intune-devices-windowsdefenderscanactionresult.md)
- [<span data-ttu-id="152d4-141">Conta do dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="152d4-141">Windows device account</span></span>](intune-devices-windowsdeviceaccount.md)
- [<span data-ttu-id="152d4-142">Conta do AD de dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="152d4-142">Windows device AD account</span></span>](intune-devices-windowsdeviceadaccount.md)
- [<span data-ttu-id="152d4-143">Conta do Azure AD de dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="152d4-143">Windows device Azure AD account</span></span>](intune-devices-windowsdeviceazureadaccount.md)
