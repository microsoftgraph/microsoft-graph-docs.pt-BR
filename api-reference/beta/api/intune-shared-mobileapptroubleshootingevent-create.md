---
title: Criar mobileAppTroubleshootingEvent
description: Descreve o método Create mobileAppTroubleshootingEvent da API do Microsoft Graph para o Intune, que oferece suporte a vários fluxos de trabalho.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9eae0c2d66dc28fd70d95c66f2ce034b16523d30
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35979747"
---
# <a name="create-mobileapptroubleshootingevent"></a><span data-ttu-id="f53e3-103">Criar mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="f53e3-103">Create mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="f53e3-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f53e3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f53e3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f53e3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f53e3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f53e3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f53e3-107">Criar um novo objeto [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="f53e3-107">Create a new [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f53e3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f53e3-108">Prerequisites</span></span>
<span data-ttu-id="f53e3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f53e3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f53e3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f53e3-111">Permission type</span></span>|<span data-ttu-id="f53e3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f53e3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f53e3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f53e3-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="f53e3-114">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="f53e3-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="f53e3-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f53e3-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f53e3-116">&nbsp; &nbsp; **Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="f53e3-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="f53e3-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f53e3-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f53e3-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f53e3-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f53e3-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f53e3-119">Not supported.</span></span>|
|<span data-ttu-id="f53e3-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f53e3-120">Application</span></span>|<span data-ttu-id="f53e3-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f53e3-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f53e3-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f53e3-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents
POST /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="f53e3-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f53e3-123">Request headers</span></span>
|<span data-ttu-id="f53e3-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f53e3-124">Header</span></span>|<span data-ttu-id="f53e3-125">Valor</span><span class="sxs-lookup"><span data-stu-id="f53e3-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f53e3-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="f53e3-126">Authorization</span></span>|<span data-ttu-id="f53e3-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f53e3-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f53e3-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f53e3-128">Accept</span></span>|<span data-ttu-id="f53e3-129">application/json</span><span class="sxs-lookup"><span data-stu-id="f53e3-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f53e3-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f53e3-130">Request body</span></span>
<span data-ttu-id="f53e3-131">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="f53e3-131">In the request body, supply a JSON representation for the mobileAppTroubleshootingEvent object.</span></span>

<span data-ttu-id="f53e3-132">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="f53e3-132">The following table shows the properties that are required when you create the mobileAppTroubleshootingEvent.</span></span>

|<span data-ttu-id="f53e3-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f53e3-133">Property</span></span>|<span data-ttu-id="f53e3-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="f53e3-134">Type</span></span>|<span data-ttu-id="f53e3-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="f53e3-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f53e3-136">id</span><span class="sxs-lookup"><span data-stu-id="f53e3-136">id</span></span>|<span data-ttu-id="f53e3-137">String</span><span class="sxs-lookup"><span data-stu-id="f53e3-137">String</span></span>|<span data-ttu-id="f53e3-138">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="f53e3-138">The GUID for the object</span></span>|
|<span data-ttu-id="f53e3-139">**Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="f53e3-139">**Troubleshooting**</span></span>|
|<span data-ttu-id="f53e3-140">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="f53e3-140">additionalInformation</span></span>|<span data-ttu-id="f53e3-141">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="f53e3-141">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="f53e3-142">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres que fornece informações adicionais sobre o evento de solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="f53e3-142">A set of string key and string value pairs which provides additional information on the Troubleshooting event.</span></span>|
|<span data-ttu-id="f53e3-143">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="f53e3-143">applicationId</span></span>|<span data-ttu-id="f53e3-144">String</span><span class="sxs-lookup"><span data-stu-id="f53e3-144">String</span></span>|<span data-ttu-id="f53e3-145">Identificador de aplicativo do Intune.</span><span class="sxs-lookup"><span data-stu-id="f53e3-145">Intune application identifier.</span></span>|
|<span data-ttu-id="f53e3-146">correlationId</span><span class="sxs-lookup"><span data-stu-id="f53e3-146">correlationId</span></span>|<span data-ttu-id="f53e3-147">String</span><span class="sxs-lookup"><span data-stu-id="f53e3-147">String</span></span>|<span data-ttu-id="f53e3-148">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="f53e3-148">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="f53e3-149">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="f53e3-149">eventDateTime</span></span>|<span data-ttu-id="f53e3-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f53e3-150">DateTimeOffset</span></span>|<span data-ttu-id="f53e3-151">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="f53e3-151">Time when the event occurred .</span></span> |
|<span data-ttu-id="f53e3-152">EventName</span><span class="sxs-lookup"><span data-stu-id="f53e3-152">eventName</span></span>|<span data-ttu-id="f53e3-153">String</span><span class="sxs-lookup"><span data-stu-id="f53e3-153">String</span></span>|<span data-ttu-id="f53e3-154">Nome do evento correspondente ao evento de solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="f53e3-154">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="f53e3-155">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f53e3-155">Optional.</span></span>|
|<span data-ttu-id="f53e3-156">histórico</span><span class="sxs-lookup"><span data-stu-id="f53e3-156">history</span></span>|<span data-ttu-id="f53e3-157">coleção [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="f53e3-157">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="f53e3-158">Item do histórico de solução de problemas do aplicativo móvel do Intune</span><span class="sxs-lookup"><span data-stu-id="f53e3-158">Intune Mobile Application Troubleshooting History Item</span></span>|
|<span data-ttu-id="f53e3-159">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="f53e3-159">managedDeviceIdentifier</span></span>|<span data-ttu-id="f53e3-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f53e3-160">String</span></span>|<span data-ttu-id="f53e3-161">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="f53e3-161">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="f53e3-162">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="f53e3-162">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="f53e3-163">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="f53e3-163">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="f53e3-164">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="f53e3-164">Object containing detailed information about the error and its remediation.</span></span> |
|<span data-ttu-id="f53e3-165">userId</span><span class="sxs-lookup"><span data-stu-id="f53e3-165">userId</span></span>|<span data-ttu-id="f53e3-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f53e3-166">String</span></span>|<span data-ttu-id="f53e3-167">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f53e3-167">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="response"></a><span data-ttu-id="f53e3-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="f53e3-168">Response</span></span>
<span data-ttu-id="f53e3-169">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f53e3-169">If successful, this method returns a `201 Created` response code and a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f53e3-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f53e3-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="f53e3-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f53e3-171">Request</span></span>
<span data-ttu-id="f53e3-172">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f53e3-172">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a><span data-ttu-id="f53e3-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="f53e3-173">Response</span></span>
<span data-ttu-id="f53e3-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f53e3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```




