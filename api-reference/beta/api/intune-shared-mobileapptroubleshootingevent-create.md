---
title: Criar mobileAppTroubleshootingEvent
description: Descreve o método Create mobileAppTroubleshootingEvent da API do Microsoft Graph para Intune, que oferece suporte a vários fluxos de trabalho.
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a42e9446892e247c47a073ce00f09102b773fb7f
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866997"
---
# <a name="create-mobileapptroubleshootingevent"></a><span data-ttu-id="cfe1e-103">Criar mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="cfe1e-103">Create mobileAppTroubleshootingEvent</span></span>

<span data-ttu-id="cfe1e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfe1e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cfe1e-105">**Importante:** APIs na versão /beta do Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cfe1e-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cfe1e-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cfe1e-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cfe1e-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cfe1e-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfe1e-108">Crie um novo [objeto mobileAppTroubleshootingEvent.](../resources/intune-shared-mobileapptroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="cfe1e-108">Create a new [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cfe1e-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cfe1e-109">Prerequisites</span></span>
<span data-ttu-id="cfe1e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfe1e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfe1e-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cfe1e-112">Permission type</span></span>|<span data-ttu-id="cfe1e-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cfe1e-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cfe1e-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cfe1e-114">Delegated (work or school account)</span></span>||
|<span data-ttu-id="cfe1e-115">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="cfe1e-115">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="cfe1e-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfe1e-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cfe1e-117">&nbsp; &nbsp; **Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="cfe1e-117">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="cfe1e-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfe1e-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cfe1e-119">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cfe1e-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cfe1e-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cfe1e-120">Not supported.</span></span>|
|<span data-ttu-id="cfe1e-121">Application</span><span class="sxs-lookup"><span data-stu-id="cfe1e-121">Application</span></span>||
|<span data-ttu-id="cfe1e-122">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="cfe1e-122">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="cfe1e-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfe1e-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cfe1e-124">&nbsp; &nbsp; **Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="cfe1e-124">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="cfe1e-125">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfe1e-125">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cfe1e-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cfe1e-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents
POST /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="cfe1e-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cfe1e-127">Request headers</span></span>
|<span data-ttu-id="cfe1e-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cfe1e-128">Header</span></span>|<span data-ttu-id="cfe1e-129">Valor</span><span class="sxs-lookup"><span data-stu-id="cfe1e-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cfe1e-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="cfe1e-130">Authorization</span></span>|<span data-ttu-id="cfe1e-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cfe1e-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cfe1e-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cfe1e-132">Accept</span></span>|<span data-ttu-id="cfe1e-133">application/json</span><span class="sxs-lookup"><span data-stu-id="cfe1e-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cfe1e-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cfe1e-134">Request body</span></span>
<span data-ttu-id="cfe1e-135">No corpo da solicitação, fornece uma representação JSON para o objeto mobileAppTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="cfe1e-135">In the request body, supply a JSON representation for the mobileAppTroubleshootingEvent object.</span></span>

<span data-ttu-id="cfe1e-136">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="cfe1e-136">The following table shows the properties that are required when you create the mobileAppTroubleshootingEvent.</span></span>

|<span data-ttu-id="cfe1e-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cfe1e-137">Property</span></span>|<span data-ttu-id="cfe1e-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="cfe1e-138">Type</span></span>|<span data-ttu-id="cfe1e-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfe1e-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfe1e-140">id</span><span class="sxs-lookup"><span data-stu-id="cfe1e-140">id</span></span>|<span data-ttu-id="cfe1e-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cfe1e-141">String</span></span>|<span data-ttu-id="cfe1e-142">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="cfe1e-142">The GUID for the object</span></span>|
|<span data-ttu-id="cfe1e-143">**Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="cfe1e-143">**Troubleshooting**</span></span>|
|<span data-ttu-id="cfe1e-144">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="cfe1e-144">additionalInformation</span></span>|<span data-ttu-id="cfe1e-145">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="cfe1e-145">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="cfe1e-146">Um conjunto de pares de valores de chave de cadeia de caracteres e cadeia de caracteres que fornece informações adicionais sobre o evento Solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="cfe1e-146">A set of string key and string value pairs which provides additional information on the Troubleshooting event.</span></span>|
|<span data-ttu-id="cfe1e-147">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="cfe1e-147">applicationId</span></span>|<span data-ttu-id="cfe1e-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cfe1e-148">String</span></span>|<span data-ttu-id="cfe1e-149">Identificador de aplicativo do Intune.</span><span class="sxs-lookup"><span data-stu-id="cfe1e-149">Intune application identifier.</span></span>|
|<span data-ttu-id="cfe1e-150">correlationId</span><span class="sxs-lookup"><span data-stu-id="cfe1e-150">correlationId</span></span>|<span data-ttu-id="cfe1e-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cfe1e-151">String</span></span>|<span data-ttu-id="cfe1e-152">ID usada para rastrear a falha no serviço.</span><span class="sxs-lookup"><span data-stu-id="cfe1e-152">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="cfe1e-153">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="cfe1e-153">eventDateTime</span></span>|<span data-ttu-id="cfe1e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfe1e-154">DateTimeOffset</span></span>|<span data-ttu-id="cfe1e-155">A hora em que o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="cfe1e-155">Time when the event occurred .</span></span> |
|<span data-ttu-id="cfe1e-156">eventName</span><span class="sxs-lookup"><span data-stu-id="cfe1e-156">eventName</span></span>|<span data-ttu-id="cfe1e-157">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="cfe1e-157">String</span></span>|<span data-ttu-id="cfe1e-158">Nome do Evento correspondente ao Evento de Solução de Problemas.</span><span class="sxs-lookup"><span data-stu-id="cfe1e-158">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="cfe1e-159">Opcional.</span><span class="sxs-lookup"><span data-stu-id="cfe1e-159">Optional.</span></span>|
|<span data-ttu-id="cfe1e-160">history</span><span class="sxs-lookup"><span data-stu-id="cfe1e-160">history</span></span>|<span data-ttu-id="cfe1e-161">[coleção mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="cfe1e-161">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="cfe1e-162">Item histórico de solução de problemas de aplicativo móvel do Intune</span><span class="sxs-lookup"><span data-stu-id="cfe1e-162">Intune Mobile Application Troubleshooting History Item</span></span>|
|<span data-ttu-id="cfe1e-163">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="cfe1e-163">managedDeviceIdentifier</span></span>|<span data-ttu-id="cfe1e-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cfe1e-164">String</span></span>|<span data-ttu-id="cfe1e-165">Identificador de dispositivo criado ou coletado pelo Intune.</span><span class="sxs-lookup"><span data-stu-id="cfe1e-165">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="cfe1e-166">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="cfe1e-166">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="cfe1e-167">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="cfe1e-167">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="cfe1e-168">Objeto contendo informações detalhadas sobre o erro e sua correção.</span><span class="sxs-lookup"><span data-stu-id="cfe1e-168">Object containing detailed information about the error and its remediation.</span></span> |
|<span data-ttu-id="cfe1e-169">userId</span><span class="sxs-lookup"><span data-stu-id="cfe1e-169">userId</span></span>|<span data-ttu-id="cfe1e-170">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cfe1e-170">String</span></span>|<span data-ttu-id="cfe1e-171">Identificador do usuário que tentou registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cfe1e-171">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="response"></a><span data-ttu-id="cfe1e-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfe1e-172">Response</span></span>
<span data-ttu-id="cfe1e-173">Se tiver êxito, este método retornará um código de `201 Created` resposta e um objeto [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cfe1e-173">If successful, this method returns a `201 Created` response code and a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfe1e-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cfe1e-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="cfe1e-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cfe1e-175">Request</span></span>
<span data-ttu-id="cfe1e-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cfe1e-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a><span data-ttu-id="cfe1e-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfe1e-177">Response</span></span>
<span data-ttu-id="cfe1e-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cfe1e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```











