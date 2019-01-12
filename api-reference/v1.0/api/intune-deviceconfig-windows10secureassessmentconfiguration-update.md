---
title: Atualizar windows10SecureAssessmentConfiguration
description: Atualizar as propriedades de um objeto windows10SecureAssessmentConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8291ca608bda0f18152999747381d3649e88f6fc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917360"
---
# <a name="update-windows10secureassessmentconfiguration"></a><span data-ttu-id="47b2e-103">Atualizar windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="47b2e-103">Update windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="47b2e-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="47b2e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47b2e-105">Atualizar as propriedades de um objeto [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47b2e-105">Update the properties of a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="47b2e-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="47b2e-106">Prerequisites</span></span>
<span data-ttu-id="47b2e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47b2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47b2e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47b2e-109">Permission type</span></span>|<span data-ttu-id="47b2e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="47b2e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47b2e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47b2e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="47b2e-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47b2e-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="47b2e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47b2e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47b2e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47b2e-114">Not supported.</span></span>|
|<span data-ttu-id="47b2e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47b2e-115">Application</span></span>|<span data-ttu-id="47b2e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47b2e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47b2e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47b2e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="47b2e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47b2e-118">Request headers</span></span>
|<span data-ttu-id="47b2e-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="47b2e-119">Header</span></span>|<span data-ttu-id="47b2e-120">Valor</span><span class="sxs-lookup"><span data-stu-id="47b2e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47b2e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="47b2e-121">Authorization</span></span>|<span data-ttu-id="47b2e-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47b2e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47b2e-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="47b2e-123">Accept</span></span>|<span data-ttu-id="47b2e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="47b2e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47b2e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47b2e-125">Request body</span></span>
<span data-ttu-id="47b2e-126">No corpo da solicitação, forneça uma representação JSON do objeto [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47b2e-126">In the request body, supply a JSON representation for the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

<span data-ttu-id="47b2e-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47b2e-127">The following table shows the properties that are required when you create the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span></span>

|<span data-ttu-id="47b2e-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="47b2e-128">Property</span></span>|<span data-ttu-id="47b2e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="47b2e-129">Type</span></span>|<span data-ttu-id="47b2e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="47b2e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47b2e-131">id</span><span class="sxs-lookup"><span data-stu-id="47b2e-131">id</span></span>|<span data-ttu-id="47b2e-132">String</span><span class="sxs-lookup"><span data-stu-id="47b2e-132">String</span></span>|<span data-ttu-id="47b2e-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="47b2e-133">Key of the entity.</span></span> <span data-ttu-id="47b2e-134">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47b2e-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47b2e-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="47b2e-135">lastModifiedDateTime</span></span>|<span data-ttu-id="47b2e-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47b2e-136">DateTimeOffset</span></span>|<span data-ttu-id="47b2e-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="47b2e-137">DateTime the object was last modified.</span></span> <span data-ttu-id="47b2e-138">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47b2e-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47b2e-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="47b2e-139">createdDateTime</span></span>|<span data-ttu-id="47b2e-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47b2e-140">DateTimeOffset</span></span>|<span data-ttu-id="47b2e-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="47b2e-141">DateTime the object was created.</span></span> <span data-ttu-id="47b2e-142">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47b2e-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47b2e-143">description</span><span class="sxs-lookup"><span data-stu-id="47b2e-143">description</span></span>|<span data-ttu-id="47b2e-144">String</span><span class="sxs-lookup"><span data-stu-id="47b2e-144">String</span></span>|<span data-ttu-id="47b2e-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="47b2e-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="47b2e-146">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47b2e-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47b2e-147">displayName</span><span class="sxs-lookup"><span data-stu-id="47b2e-147">displayName</span></span>|<span data-ttu-id="47b2e-148">String</span><span class="sxs-lookup"><span data-stu-id="47b2e-148">String</span></span>|<span data-ttu-id="47b2e-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="47b2e-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="47b2e-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47b2e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47b2e-151">version</span><span class="sxs-lookup"><span data-stu-id="47b2e-151">version</span></span>|<span data-ttu-id="47b2e-152">Int32</span><span class="sxs-lookup"><span data-stu-id="47b2e-152">Int32</span></span>|<span data-ttu-id="47b2e-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="47b2e-153">Version of the device configuration.</span></span> <span data-ttu-id="47b2e-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47b2e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47b2e-155">launchUri</span><span class="sxs-lookup"><span data-stu-id="47b2e-155">launchUri</span></span>|<span data-ttu-id="47b2e-156">String</span><span class="sxs-lookup"><span data-stu-id="47b2e-156">String</span></span>|<span data-ttu-id="47b2e-157">Link da URL para uma avaliação que é carregada automaticamente quando o navegador de avaliação segura é iniciado.</span><span class="sxs-lookup"><span data-stu-id="47b2e-157">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="47b2e-158">Ele precisa ser uma URL válida (http\[s\]://msdn.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="47b2e-158">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="47b2e-159">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="47b2e-159">configurationAccount</span></span>|<span data-ttu-id="47b2e-160">String</span><span class="sxs-lookup"><span data-stu-id="47b2e-160">String</span></span>|<span data-ttu-id="47b2e-161">A conta usada para configurar o dispositivo Windows para realizar o teste.</span><span class="sxs-lookup"><span data-stu-id="47b2e-161">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="47b2e-162">O usuário pode ser uma conta de domínio (domínio\usuário), uma conta do AAD (nomedeusuário@locatário.com) ou uma conta local (nomedeusuário).</span><span class="sxs-lookup"><span data-stu-id="47b2e-162">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="47b2e-163">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="47b2e-163">allowPrinting</span></span>|<span data-ttu-id="47b2e-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="47b2e-164">Boolean</span></span>|<span data-ttu-id="47b2e-165">Indica se o aplicativo deve ou não ter permissão de impressão durante o teste.</span><span class="sxs-lookup"><span data-stu-id="47b2e-165">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="47b2e-166">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="47b2e-166">allowScreenCapture</span></span>|<span data-ttu-id="47b2e-167">Booliano</span><span class="sxs-lookup"><span data-stu-id="47b2e-167">Boolean</span></span>|<span data-ttu-id="47b2e-168">Indica se a capacidade de captura de tela deve ou não ser permitida durante um teste.</span><span class="sxs-lookup"><span data-stu-id="47b2e-168">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="47b2e-169">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="47b2e-169">allowTextSuggestion</span></span>|<span data-ttu-id="47b2e-170">Booliano</span><span class="sxs-lookup"><span data-stu-id="47b2e-170">Boolean</span></span>|<span data-ttu-id="47b2e-171">Indica se sugestões de texto devem ou não ser permitidas durante o teste.</span><span class="sxs-lookup"><span data-stu-id="47b2e-171">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="47b2e-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="47b2e-172">Response</span></span>
<span data-ttu-id="47b2e-173">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47b2e-173">If successful, this method returns a `200 OK` response code and an updated [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47b2e-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47b2e-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="47b2e-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47b2e-175">Request</span></span>
<span data-ttu-id="47b2e-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47b2e-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 359

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```

### <a name="response"></a><span data-ttu-id="47b2e-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="47b2e-177">Response</span></span>
<span data-ttu-id="47b2e-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="47b2e-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 531

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "id": "f60d71be-71be-f60d-be71-0df6be710df6",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```



