---
title: Criar mobileAppTroubleshootingEvent
description: Descreve o método de mobileAppTroubleshootingEvent Create da API Microsoft Graph para Intune, que oferece suporte a vários fluxos de trabalho.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e409aa663ff2471222a7e36a9e381505792f37eb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431276"
---
# <a name="create-mobileapptroubleshootingevent"></a><span data-ttu-id="66a9f-103">Criar mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="66a9f-103">Create mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="66a9f-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="66a9f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="66a9f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="66a9f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="66a9f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="66a9f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66a9f-107">Crie um novo objeto de [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="66a9f-107">Create a new [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66a9f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="66a9f-108">Prerequisites</span></span>
<span data-ttu-id="66a9f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="66a9f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="66a9f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66a9f-111">Permission type</span></span>|<span data-ttu-id="66a9f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="66a9f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66a9f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66a9f-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="66a9f-114">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="66a9f-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="66a9f-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66a9f-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="66a9f-116">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="66a9f-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="66a9f-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66a9f-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="66a9f-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66a9f-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66a9f-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66a9f-119">Not supported.</span></span>|
|<span data-ttu-id="66a9f-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66a9f-120">Application</span></span>|<span data-ttu-id="66a9f-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66a9f-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66a9f-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66a9f-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents
POST /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="66a9f-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66a9f-123">Request headers</span></span>
|<span data-ttu-id="66a9f-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="66a9f-124">Header</span></span>|<span data-ttu-id="66a9f-125">Valor</span><span class="sxs-lookup"><span data-stu-id="66a9f-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66a9f-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="66a9f-126">Authorization</span></span>|<span data-ttu-id="66a9f-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66a9f-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66a9f-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="66a9f-128">Accept</span></span>|<span data-ttu-id="66a9f-129">application/json</span><span class="sxs-lookup"><span data-stu-id="66a9f-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66a9f-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66a9f-130">Request body</span></span>
<span data-ttu-id="66a9f-131">No corpo da solicitação, fornece uma representação JSON para o objeto mobileAppTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="66a9f-131">In the request body, supply a JSON representation for the mobileAppTroubleshootingEvent object.</span></span>

<span data-ttu-id="66a9f-132">A tabela a seguir mostra as propriedades que são necessárias quando você cria o mobileAppTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="66a9f-132">The following table shows the properties that are required when you create the mobileAppTroubleshootingEvent.</span></span>

|<span data-ttu-id="66a9f-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66a9f-133">Property</span></span>|<span data-ttu-id="66a9f-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="66a9f-134">Type</span></span>|<span data-ttu-id="66a9f-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="66a9f-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66a9f-136">id</span><span class="sxs-lookup"><span data-stu-id="66a9f-136">id</span></span>|<span data-ttu-id="66a9f-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66a9f-137">String</span></span>|<span data-ttu-id="66a9f-138">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="66a9f-138">The GUID for the object</span></span>|
|<span data-ttu-id="66a9f-139">**Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="66a9f-139">**Troubleshooting**</span></span>|
|<span data-ttu-id="66a9f-140">informações adicionais</span><span class="sxs-lookup"><span data-stu-id="66a9f-140">additionalInformation</span></span>|<span data-ttu-id="66a9f-141">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="66a9f-141">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="66a9f-142">Um conjunto de chave de cadeia de caracteres e pares de valor de cadeia de caracteres que fornece informações adicionais sobre o evento de solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="66a9f-142">A set of string key and string value pairs which provides additional information on the Troubleshooting event.</span></span>|
|<span data-ttu-id="66a9f-143">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="66a9f-143">applicationId</span></span>|<span data-ttu-id="66a9f-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66a9f-144">String</span></span>|<span data-ttu-id="66a9f-145">Identificador de aplicativo Intune.</span><span class="sxs-lookup"><span data-stu-id="66a9f-145">Intune application identifier.</span></span>|
|<span data-ttu-id="66a9f-146">correlationId</span><span class="sxs-lookup"><span data-stu-id="66a9f-146">correlationId</span></span>|<span data-ttu-id="66a9f-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66a9f-147">String</span></span>|<span data-ttu-id="66a9f-148">ID usado para a falha no serviço de rastreamento.</span><span class="sxs-lookup"><span data-stu-id="66a9f-148">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="66a9f-149">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="66a9f-149">eventDateTime</span></span>|<span data-ttu-id="66a9f-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66a9f-150">DateTimeOffset</span></span>|<span data-ttu-id="66a9f-151">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="66a9f-151">Time when the event occurred .</span></span> |
|<span data-ttu-id="66a9f-152">eventName</span><span class="sxs-lookup"><span data-stu-id="66a9f-152">eventName</span></span>|<span data-ttu-id="66a9f-153">String</span><span class="sxs-lookup"><span data-stu-id="66a9f-153">String</span></span>|<span data-ttu-id="66a9f-154">Nome do evento correspondente ao evento de solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="66a9f-154">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="66a9f-155">Opcional.</span><span class="sxs-lookup"><span data-stu-id="66a9f-155">Optional.</span></span>|
|<span data-ttu-id="66a9f-156">histórico</span><span class="sxs-lookup"><span data-stu-id="66a9f-156">history</span></span>|<span data-ttu-id="66a9f-157">coleção [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="66a9f-157">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="66a9f-158">Aplicativo móvel Intune Item do histórico de solução de problemas</span><span class="sxs-lookup"><span data-stu-id="66a9f-158">Intune Mobile Application Troubleshooting History Item</span></span>|
|<span data-ttu-id="66a9f-159">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="66a9f-159">managedDeviceIdentifier</span></span>|<span data-ttu-id="66a9f-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66a9f-160">String</span></span>|<span data-ttu-id="66a9f-161">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="66a9f-161">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="66a9f-162">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="66a9f-162">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="66a9f-163">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="66a9f-163">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="66a9f-164">Objeto que contém informações detalhadas sobre o erro e suas atualizações.</span><span class="sxs-lookup"><span data-stu-id="66a9f-164">Object containing detailed information about the error and its remediation.</span></span> |
|<span data-ttu-id="66a9f-165">userId</span><span class="sxs-lookup"><span data-stu-id="66a9f-165">userId</span></span>|<span data-ttu-id="66a9f-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66a9f-166">String</span></span>|<span data-ttu-id="66a9f-167">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66a9f-167">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="response"></a><span data-ttu-id="66a9f-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="66a9f-168">Response</span></span>
<span data-ttu-id="66a9f-169">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66a9f-169">If successful, this method returns a `201 Created` response code and a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66a9f-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66a9f-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="66a9f-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66a9f-171">Request</span></span>
<span data-ttu-id="66a9f-172">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="66a9f-172">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a><span data-ttu-id="66a9f-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="66a9f-173">Response</span></span>
<span data-ttu-id="66a9f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="66a9f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```




