---
title: Gerenciamento de dispositivos no Microsoft Intune
description: Recursos de gerenciamento de dispositivos no Microsoft Intune
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 426b3f8cc3f21547cec191afbfb954bf37e6969a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449393"
---
# <a name="device-management-in-microsoft-intune"></a><span data-ttu-id="5da31-103">Gerenciamento de dispositivos no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="5da31-103">Device management in Microsoft Intune</span></span>

<span data-ttu-id="5da31-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5da31-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5da31-105">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5da31-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

- [<span data-ttu-id="5da31-106">Estado da ação</span><span class="sxs-lookup"><span data-stu-id="5da31-106">Action state</span></span>](intune-devices-actionstate.md)
- [<span data-ttu-id="5da31-107">Certificado de notificação por push da Apple</span><span class="sxs-lookup"><span data-stu-id="5da31-107">Apple push notification certificate</span></span>](intune-devices-applepushnotificationcertificate.md)
- [<span data-ttu-id="5da31-108">Ator de auditoria</span><span class="sxs-lookup"><span data-stu-id="5da31-108">Audit actor</span></span>](intune-auditing-auditactor.md)
- [<span data-ttu-id="5da31-109">Evento de auditoria</span><span class="sxs-lookup"><span data-stu-id="5da31-109">Audit event</span></span>](intune-auditing-auditevent.md)
- [<span data-ttu-id="5da31-110">Propriedade de auditoria</span><span class="sxs-lookup"><span data-stu-id="5da31-110">Audit property</span></span>](intune-auditing-auditproperty.md)
- [<span data-ttu-id="5da31-111">Recurso de auditoria</span><span class="sxs-lookup"><span data-stu-id="5da31-111">Audit resource</span></span>](intune-auditing-auditresource.md)
- [<span data-ttu-id="5da31-112">Estado de conformidade</span><span class="sxs-lookup"><span data-stu-id="5da31-112">Compliance state</span></span>](intune-devices-compliancestate.md)
- [<span data-ttu-id="5da31-113">Recursos habilitados pelo cliente do Gerenciador de Configurações</span><span class="sxs-lookup"><span data-stu-id="5da31-113">Configuration manager client enabled features</span></span>](intune-devices-configurationmanagerclientenabledfeatures.md)
- [<span data-ttu-id="5da31-114">Resultado da ação de excluir o usuário do dispositivo compartilhado da Apple</span><span class="sxs-lookup"><span data-stu-id="5da31-114">Delete user from shared Apple device action result</span></span>](intune-devices-deleteuserfromsharedappledeviceactionresult.md)
- [<span data-ttu-id="5da31-115">Aplicativo detectado</span><span class="sxs-lookup"><span data-stu-id="5da31-115">Detected app</span></span>](intune-devices-detectedapp.md)
- [<span data-ttu-id="5da31-116">Resultado da ação do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5da31-116">Device action result</span></span>](intune-devices-deviceactionresult.md)
- [<span data-ttu-id="5da31-117">Motivo da falha de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5da31-117">Device enrollment failure reason</span></span>](intune-troubleshooting-deviceenrollmentfailurereason.md)
- [<span data-ttu-id="5da31-118">Resumo do Estado de Acesso ao Exchange do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5da31-118">Device exchange access state summary</span></span>](intune-devices-deviceexchangeaccessstatesummary.md)
- [<span data-ttu-id="5da31-119">Geolocalização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5da31-119">Device geolocation</span></span>](intune-devices-devicegeolocation.md)
- [<span data-ttu-id="5da31-120">Estado do atestado de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5da31-120">Device health attestation state</span></span>](intune-devices-devicehealthattestationstate.md)
- [<span data-ttu-id="5da31-121">Estado de acesso do Exchange de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="5da31-121">Device management exchange access state</span></span>](intune-devices-devicemanagementexchangeaccessstate.md)
- [<span data-ttu-id="5da31-122">Motivo do estado de acesso do Exchange de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="5da31-122">Device management exchange access state reason</span></span>](intune-devices-devicemanagementexchangeaccessstatereason.md)
- [<span data-ttu-id="5da31-123">Estado de assinatura de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="5da31-123">Device management subscription state</span></span>](intune-devices-devicemanagementsubscriptionstate.md)
- [<span data-ttu-id="5da31-124">Evento de solução de problemas com o gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="5da31-124">Device management troubleshooting event</span></span>](intune-troubleshooting-devicemanagementtroubleshootingevent.md)
- [<span data-ttu-id="5da31-125">Resumo do sistema operacional do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5da31-125">Device operating system summary</span></span>](intune-devices-deviceoperatingsystemsummary.md)
- [<span data-ttu-id="5da31-126">Estado do registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5da31-126">Device registration state</span></span>](intune-devices-deviceregistrationstate.md)
- [<span data-ttu-id="5da31-127">Evento de solução de problemas de registro</span><span class="sxs-lookup"><span data-stu-id="5da31-127">Enrollment troubleshooting event</span></span>](intune-troubleshooting-enrollmenttroubleshootingevent.md)
- [<span data-ttu-id="5da31-128">Mensagem de notificação localizada</span><span class="sxs-lookup"><span data-stu-id="5da31-128">Localized notification message</span></span>](intune-notification-localizednotificationmessage.md)
- [<span data-ttu-id="5da31-129">Resultado da ação de localizar dispositivo</span><span class="sxs-lookup"><span data-stu-id="5da31-129">Locate device action result</span></span>](intune-devices-locatedeviceactionresult.md)
- [<span data-ttu-id="5da31-130">Dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="5da31-130">Managed device</span></span>](intune-devices-manageddevice.md)
- [<span data-ttu-id="5da31-131">Visão geral do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="5da31-131">Managed device overview</span></span>](intune-devices-manageddeviceoverview.md)
- [<span data-ttu-id="5da31-132">Tipo de proprietário do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="5da31-132">Managed device owner type</span></span>](intune-devices-manageddeviceownertype.md)
- [<span data-ttu-id="5da31-133">Estado de integridade reportado pelo parceiro do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="5da31-133">Managed device partner reported health state</span></span>](intune-devices-manageddevicepartnerreportedhealthstate.md)
- [<span data-ttu-id="5da31-134">Tipo de agente de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="5da31-134">Management agent type</span></span>](intune-devices-managementagenttype.md)
- [<span data-ttu-id="5da31-135">Modelo de mensagem de notificação</span><span class="sxs-lookup"><span data-stu-id="5da31-135">Notification message template</span></span>](intune-notification-notificationmessagetemplate.md)
- [<span data-ttu-id="5da31-136">Opções de identidade visual do modelo de notificação</span><span class="sxs-lookup"><span data-stu-id="5da31-136">Notification template branding options</span></span>](intune-notification-notificationtemplatebrandingoptions.md)
- [<span data-ttu-id="5da31-137">Status da inclusão de assistência remota</span><span class="sxs-lookup"><span data-stu-id="5da31-137">Remote assistance on-boarding status</span></span>](intune-remoteassistance-remoteassistanceonboardingstatus.md)
- [<span data-ttu-id="5da31-138">Parceiro de assistência remota</span><span class="sxs-lookup"><span data-stu-id="5da31-138">Remote assistance partner</span></span>](intune-remoteassistance-remoteassistancepartner.md)
- [<span data-ttu-id="5da31-139">Resultado da ação de bloqueio remoto</span><span class="sxs-lookup"><span data-stu-id="5da31-139">Remote lock action result</span></span>](intune-devices-remotelockactionresult.md)
- [<span data-ttu-id="5da31-140">Resultado da ação de redefinir a senha</span><span class="sxs-lookup"><span data-stu-id="5da31-140">Reset passcode action result</span></span>](intune-devices-resetpasscodeactionresult.md)
- [<span data-ttu-id="5da31-141">Parâmetro da ação de atualização de conta de dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="5da31-141">Update windows device account action parameter</span></span>](intune-devices-updatewindowsdeviceaccountactionparameter.md)
- [<span data-ttu-id="5da31-142">Resultado da ação de verificação do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="5da31-142">Windows defender scan action result</span></span>](intune-devices-windowsdefenderscanactionresult.md)
- [<span data-ttu-id="5da31-143">Conta do dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="5da31-143">Windows device account</span></span>](intune-devices-windowsdeviceaccount.md)
- [<span data-ttu-id="5da31-144">Conta do AD de dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="5da31-144">Windows device AD account</span></span>](intune-devices-windowsdeviceadaccount.md)
- [<span data-ttu-id="5da31-145">Conta do Azure AD de dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="5da31-145">Windows device Azure AD account</span></span>](intune-devices-windowsdeviceazureadaccount.md)




