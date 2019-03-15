---
title: Atualizar deviceManagement
description: Atualizar as propriedades de um objeto deviceManagement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a71212652d789b08a8cb496b6b98c18b12d3e9c7
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571050"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="4de2c-103">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="4de2c-103">Update deviceManagement</span></span>

> <span data-ttu-id="4de2c-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4de2c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4de2c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4de2c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4de2c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4de2c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4de2c-107">Atualizar as propriedades de um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="4de2c-107">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4de2c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4de2c-108">Prerequisites</span></span>

<span data-ttu-id="4de2c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4de2c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

<span data-ttu-id="4de2c-111">Observe que a permissão varia de acordo com o fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="4de2c-111">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="4de2c-112">Tipo&nbsp;&nbsp;de permissão (&nbsp;por fluxo de trabalho)</span><span class="sxs-lookup"><span data-stu-id="4de2c-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="4de2c-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4de2c-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="4de2c-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4de2c-114">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="4de2c-115">&nbsp;&nbsp; **Android para trabalho**</span><span class="sxs-lookup"><span data-stu-id="4de2c-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="4de2c-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4de2c-116">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="4de2c-117">&nbsp; &nbsp; **Auditoria**</span><span class="sxs-lookup"><span data-stu-id="4de2c-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="4de2c-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4de2c-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="4de2c-119">&nbsp; &nbsp; **Termos da empresa**</span><span class="sxs-lookup"><span data-stu-id="4de2c-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="4de2c-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4de2c-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="4de2c-121">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="4de2c-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="4de2c-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4de2c-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="4de2c-123">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="4de2c-123">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="4de2c-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4de2c-124">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="4de2c-125">&nbsp;&nbsp; **Sim eletrônico**</span><span class="sxs-lookup"><span data-stu-id="4de2c-125">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="4de2c-126">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4de2c-126">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="4de2c-127">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="4de2c-127">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="4de2c-128">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4de2c-128">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="4de2c-129">&nbsp;&nbsp; **Isolamento**</span><span class="sxs-lookup"><span data-stu-id="4de2c-129">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="4de2c-130">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4de2c-130">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="4de2c-131">&nbsp; &nbsp; **Notificação**</span><span class="sxs-lookup"><span data-stu-id="4de2c-131">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="4de2c-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4de2c-132">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="4de2c-133">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="4de2c-133">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="4de2c-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4de2c-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="4de2c-135">&nbsp; &nbsp; **RBAC (Controle de acesso baseado na função)**</span><span class="sxs-lookup"><span data-stu-id="4de2c-135">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="4de2c-136">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4de2c-136">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="4de2c-137">&nbsp;&nbsp; **Acesso remoto**</span><span class="sxs-lookup"><span data-stu-id="4de2c-137">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="4de2c-138">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4de2c-138">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="4de2c-139">&nbsp;&nbsp; **Assistência remota**</span><span class="sxs-lookup"><span data-stu-id="4de2c-139">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="4de2c-140">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4de2c-140">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="4de2c-141">&nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações**</span><span class="sxs-lookup"><span data-stu-id="4de2c-141">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="4de2c-142">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4de2c-142">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="4de2c-143">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="4de2c-143">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="4de2c-144">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4de2c-144">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="4de2c-145">&nbsp;&nbsp; **Proteção de informações do Windows**</span><span class="sxs-lookup"><span data-stu-id="4de2c-145">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="4de2c-146">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4de2c-146">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="4de2c-147">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4de2c-147">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4de2c-148">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4de2c-148">Not supported.</span></span>|
| <span data-ttu-id="4de2c-149">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4de2c-149">Application</span></span> | <span data-ttu-id="4de2c-150">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4de2c-150">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4de2c-151">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4de2c-151">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="4de2c-152">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4de2c-152">Request headers</span></span>

|<span data-ttu-id="4de2c-153">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4de2c-153">Header</span></span>|<span data-ttu-id="4de2c-154">Valor</span><span class="sxs-lookup"><span data-stu-id="4de2c-154">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4de2c-155">Autorização</span><span class="sxs-lookup"><span data-stu-id="4de2c-155">Authorization</span></span>|<span data-ttu-id="4de2c-156">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4de2c-156">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4de2c-157">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4de2c-157">Accept</span></span>|<span data-ttu-id="4de2c-158">application/json</span><span class="sxs-lookup"><span data-stu-id="4de2c-158">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4de2c-159">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4de2c-159">Request body</span></span>

<span data-ttu-id="4de2c-160">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="4de2c-160">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="4de2c-161">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="4de2c-161">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="4de2c-162">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4de2c-162">Property</span></span>|<span data-ttu-id="4de2c-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="4de2c-163">Type</span></span>|<span data-ttu-id="4de2c-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="4de2c-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4de2c-165">id</span><span class="sxs-lookup"><span data-stu-id="4de2c-165">id</span></span>|<span data-ttu-id="4de2c-166">String</span><span class="sxs-lookup"><span data-stu-id="4de2c-166">String</span></span>|<span data-ttu-id="4de2c-167">Identificador exclusivo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4de2c-167">Unique identifier for the device.</span></span>|
|<span data-ttu-id="4de2c-168">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="4de2c-168">**Device configuration**</span></span>|
|<span data-ttu-id="4de2c-169">intuneAccountId</span><span class="sxs-lookup"><span data-stu-id="4de2c-169">intuneAccountId</span></span>|<span data-ttu-id="4de2c-170">GUID</span><span class="sxs-lookup"><span data-stu-id="4de2c-170">GUID</span></span>|<span data-ttu-id="4de2c-171">ID da conta do Intune para determinado locatário</span><span class="sxs-lookup"><span data-stu-id="4de2c-171">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="4de2c-172">legacyPcManangementEnabled</span><span class="sxs-lookup"><span data-stu-id="4de2c-172">legacyPcManangementEnabled</span></span>|<span data-ttu-id="4de2c-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="4de2c-173">Boolean</span></span>|<span data-ttu-id="4de2c-174">A propriedade para habilitar o gerenciamento de computador herdado não MDM gerenciado para esta conta.</span><span class="sxs-lookup"><span data-stu-id="4de2c-174">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="4de2c-175">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4de2c-175">This property is read-only.</span></span>|
|<span data-ttu-id="4de2c-176">maximumDepTokens</span><span class="sxs-lookup"><span data-stu-id="4de2c-176">maximumDepTokens</span></span>|<span data-ttu-id="4de2c-177">Int32</span><span class="sxs-lookup"><span data-stu-id="4de2c-177">Int32</span></span>|<span data-ttu-id="4de2c-178">Número máximo de tokens DEP permitidos por locatário.</span><span class="sxs-lookup"><span data-stu-id="4de2c-178">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="4de2c-179">settings</span><span class="sxs-lookup"><span data-stu-id="4de2c-179">settings</span></span>|[<span data-ttu-id="4de2c-180">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="4de2c-180">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="4de2c-181">Configurações de nível da conta.</span><span class="sxs-lookup"><span data-stu-id="4de2c-181">Account level settings.</span></span>|
|<span data-ttu-id="4de2c-182">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="4de2c-182">**Device management**</span></span>|
|<span data-ttu-id="4de2c-183">accountMoveCompletionDateTime</span><span class="sxs-lookup"><span data-stu-id="4de2c-183">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="4de2c-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4de2c-184">DateTimeOffset</span></span>|<span data-ttu-id="4de2c-185">A data & hora em que os dados do locatário são movidos entre ScaleUnits.</span><span class="sxs-lookup"><span data-stu-id="4de2c-185">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="4de2c-186">adminConsent</span><span class="sxs-lookup"><span data-stu-id="4de2c-186">adminConsent</span></span>|[<span data-ttu-id="4de2c-187">adminConsent</span><span class="sxs-lookup"><span data-stu-id="4de2c-187">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="4de2c-188">Informações de consentimento do administrador.</span><span class="sxs-lookup"><span data-stu-id="4de2c-188">Admin consent information.</span></span>|
|<span data-ttu-id="4de2c-189">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="4de2c-189">deviceProtectionOverview</span></span>|[<span data-ttu-id="4de2c-190">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="4de2c-190">deviceProtectionOverview</span></span>](../resources/intune-devices-deviceprotectionoverview.md)|<span data-ttu-id="4de2c-191">Visão geral da proteção de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4de2c-191">Device protection overview.</span></span>|
|<span data-ttu-id="4de2c-192">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="4de2c-192">managedDeviceCleanupSettings</span></span>|[<span data-ttu-id="4de2c-193">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="4de2c-193">managedDeviceCleanupSettings</span></span>](../resources/intune-devices-manageddevicecleanupsettings.md)|<span data-ttu-id="4de2c-194">Regra de limpeza de dispositivo</span><span class="sxs-lookup"><span data-stu-id="4de2c-194">Device cleanup rule</span></span>|
|<span data-ttu-id="4de2c-195">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="4de2c-195">subscriptionState</span></span>|[<span data-ttu-id="4de2c-196">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="4de2c-196">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="4de2c-197">Estado de assinatura de gerenciamento de dispositivo móvel do locatário.</span><span class="sxs-lookup"><span data-stu-id="4de2c-197">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="4de2c-198">Os valores possíveis são: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="4de2c-198">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="4de2c-199">assinaturas</span><span class="sxs-lookup"><span data-stu-id="4de2c-199">subscriptions</span></span>|[<span data-ttu-id="4de2c-200">deviceManagementSubscriptions</span><span class="sxs-lookup"><span data-stu-id="4de2c-200">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="4de2c-201">Assinatura do locatário.</span><span class="sxs-lookup"><span data-stu-id="4de2c-201">Tenant's Subscription.</span></span> <span data-ttu-id="4de2c-202">Os valores possíveis são: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span><span class="sxs-lookup"><span data-stu-id="4de2c-202">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="4de2c-203">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="4de2c-203">windowsMalwareOverview</span></span>|[<span data-ttu-id="4de2c-204">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="4de2c-204">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="4de2c-205">Visão geral de malware para dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="4de2c-205">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="4de2c-206">**Integração**</span><span class="sxs-lookup"><span data-stu-id="4de2c-206">**Onboarding**</span></span>|
|<span data-ttu-id="4de2c-207">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="4de2c-207">intuneBrand</span></span>|[<span data-ttu-id="4de2c-208">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="4de2c-208">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="4de2c-209">intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.</span><span class="sxs-lookup"><span data-stu-id="4de2c-209">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="4de2c-210">O suporte à propriedade do corpo da solicitação varia de acordo com o fluxo de trabalho</span><span class="sxs-lookup"><span data-stu-id="4de2c-210">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="4de2c-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="4de2c-211">Response</span></span>
<span data-ttu-id="4de2c-212">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4de2c-212">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4de2c-213">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4de2c-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="4de2c-214">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4de2c-214">Request</span></span>

<span data-ttu-id="4de2c-215">Veja a seguir um exemplo de uma solicitação após o fluxo de trabalho de gerenciamento de dispositivos:</span><span class="sxs-lookup"><span data-stu-id="4de2c-215">Here is an example of a request following the device management workflow:</span></span>

``` http
PATCH https://graph.microsoft.com/beta/deviceManagement
Content-type: application/json
Content-length: 751

{
  "subscriptionState": "active",
  "subscriptions": "intune",
  "adminConsent": {
    "@odata.type": "microsoft.graph.adminConsent",
    "shareAPNSData": "granted"
  },
  "deviceProtectionOverview": {
    "@odata.type": "microsoft.graph.deviceProtectionOverview",
    "totalReportedDeviceCount": 8,
    "inactiveThreatAgentDeviceCount": 14,
    "unknownStateThreatAgentDeviceCount": 2,
    "pendingSignatureUpdateDeviceCount": 1,
    "cleanDeviceCount": 0,
    "pendingFullScanDeviceCount": 10,
    "pendingRestartDeviceCount": 9,
    "pendingManualStepsDeviceCount": 13,
    "pendingOfflineScanDeviceCount": 13,
    "criticalFailuresDeviceCount": 11
  },
  "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
}
```

### <a name="response"></a><span data-ttu-id="4de2c-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="4de2c-216">Response</span></span>

<span data-ttu-id="4de2c-217">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4de2c-217">Here is an example of the response.</span></span> 

<span data-ttu-id="4de2c-218">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="4de2c-218">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4de2c-219">As propriedades retornadas variam de acordo com o fluxo de trabalho e o contexto.</span><span class="sxs-lookup"><span data-stu-id="4de2c-219">Returned properties vary according to workflow and context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 855

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "0b283420-3420-0b28-2034-280b2034280b",
  "subscriptionState": "active",
  "subscriptions": "intune",
  "adminConsent": {
    "@odata.type": "microsoft.graph.adminConsent",
    "shareAPNSData": "granted"
  },
  "deviceProtectionOverview": {
    "@odata.type": "microsoft.graph.deviceProtectionOverview",
    "totalReportedDeviceCount": 8,
    "inactiveThreatAgentDeviceCount": 14,
    "unknownStateThreatAgentDeviceCount": 2,
    "pendingSignatureUpdateDeviceCount": 1,
    "cleanDeviceCount": 0,
    "pendingFullScanDeviceCount": 10,
    "pendingRestartDeviceCount": 9,
    "pendingManualStepsDeviceCount": 13,
    "pendingOfflineScanDeviceCount": 13,
    "criticalFailuresDeviceCount": 11
  },
  "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
}
```



