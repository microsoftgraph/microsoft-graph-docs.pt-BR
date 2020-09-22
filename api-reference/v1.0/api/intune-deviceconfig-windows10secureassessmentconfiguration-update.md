---
title: Atualizar windows10SecureAssessmentConfiguration
description: Atualizar as propriedades de um objeto windows10SecureAssessmentConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0a1b635b259d732788021a856385fd8ffbf89189
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48045744"
---
# <a name="update-windows10secureassessmentconfiguration"></a><span data-ttu-id="b2cff-103">Atualizar windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="b2cff-103">Update windows10SecureAssessmentConfiguration</span></span>

<span data-ttu-id="b2cff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2cff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2cff-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b2cff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2cff-106">Atualizar as propriedades de um objeto [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b2cff-106">Update the properties of a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2cff-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b2cff-107">Prerequisites</span></span>
<span data-ttu-id="b2cff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2cff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2cff-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2cff-110">Permission type</span></span>|<span data-ttu-id="b2cff-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b2cff-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2cff-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2cff-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b2cff-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2cff-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b2cff-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2cff-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2cff-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2cff-115">Not supported.</span></span>|
|<span data-ttu-id="b2cff-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2cff-116">Application</span></span>|<span data-ttu-id="b2cff-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2cff-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2cff-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2cff-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b2cff-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2cff-119">Request headers</span></span>
|<span data-ttu-id="b2cff-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b2cff-120">Header</span></span>|<span data-ttu-id="b2cff-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b2cff-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2cff-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2cff-122">Authorization</span></span>|<span data-ttu-id="b2cff-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2cff-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2cff-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b2cff-124">Accept</span></span>|<span data-ttu-id="b2cff-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b2cff-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2cff-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2cff-126">Request body</span></span>
<span data-ttu-id="b2cff-127">No corpo da solicitação, forneça uma representação JSON do objeto [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b2cff-127">In the request body, supply a JSON representation for the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

<span data-ttu-id="b2cff-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b2cff-128">The following table shows the properties that are required when you create the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span></span>

|<span data-ttu-id="b2cff-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2cff-129">Property</span></span>|<span data-ttu-id="b2cff-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2cff-130">Type</span></span>|<span data-ttu-id="b2cff-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2cff-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2cff-132">id</span><span class="sxs-lookup"><span data-stu-id="b2cff-132">id</span></span>|<span data-ttu-id="b2cff-133">String</span><span class="sxs-lookup"><span data-stu-id="b2cff-133">String</span></span>|<span data-ttu-id="b2cff-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b2cff-134">Key of the entity.</span></span> <span data-ttu-id="b2cff-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2cff-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2cff-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b2cff-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b2cff-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2cff-137">DateTimeOffset</span></span>|<span data-ttu-id="b2cff-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b2cff-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b2cff-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2cff-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2cff-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b2cff-140">createdDateTime</span></span>|<span data-ttu-id="b2cff-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2cff-141">DateTimeOffset</span></span>|<span data-ttu-id="b2cff-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b2cff-142">DateTime the object was created.</span></span> <span data-ttu-id="b2cff-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2cff-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2cff-144">description</span><span class="sxs-lookup"><span data-stu-id="b2cff-144">description</span></span>|<span data-ttu-id="b2cff-145">String</span><span class="sxs-lookup"><span data-stu-id="b2cff-145">String</span></span>|<span data-ttu-id="b2cff-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2cff-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b2cff-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2cff-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2cff-148">displayName</span><span class="sxs-lookup"><span data-stu-id="b2cff-148">displayName</span></span>|<span data-ttu-id="b2cff-149">String</span><span class="sxs-lookup"><span data-stu-id="b2cff-149">String</span></span>|<span data-ttu-id="b2cff-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2cff-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b2cff-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2cff-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2cff-152">versão</span><span class="sxs-lookup"><span data-stu-id="b2cff-152">version</span></span>|<span data-ttu-id="b2cff-153">Int32</span><span class="sxs-lookup"><span data-stu-id="b2cff-153">Int32</span></span>|<span data-ttu-id="b2cff-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2cff-154">Version of the device configuration.</span></span> <span data-ttu-id="b2cff-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2cff-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2cff-156">launchUri</span><span class="sxs-lookup"><span data-stu-id="b2cff-156">launchUri</span></span>|<span data-ttu-id="b2cff-157">String</span><span class="sxs-lookup"><span data-stu-id="b2cff-157">String</span></span>|<span data-ttu-id="b2cff-158">Link de URL para uma avaliação que é carregada automaticamente quando o navegador de avaliação segura é iniciado.</span><span class="sxs-lookup"><span data-stu-id="b2cff-158">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="b2cff-159">Ele precisa ser um URL válido (http\[s\]://msdn.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="b2cff-159">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="b2cff-160">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="b2cff-160">configurationAccount</span></span>|<span data-ttu-id="b2cff-161">String</span><span class="sxs-lookup"><span data-stu-id="b2cff-161">String</span></span>|<span data-ttu-id="b2cff-162">A conta usada para configurar o dispositivo Windows para realizar o teste.</span><span class="sxs-lookup"><span data-stu-id="b2cff-162">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="b2cff-163">O usuário pode ser uma conta de domínio (domínio\usuário), uma conta do AAD (nomedeusuário@locatário.com) ou uma conta local (nomedeusuário).</span><span class="sxs-lookup"><span data-stu-id="b2cff-163">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="b2cff-164">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="b2cff-164">allowPrinting</span></span>|<span data-ttu-id="b2cff-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2cff-165">Boolean</span></span>|<span data-ttu-id="b2cff-166">Indica se o aplicativo deve ou não ter permissão de impressão durante o teste.</span><span class="sxs-lookup"><span data-stu-id="b2cff-166">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="b2cff-167">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="b2cff-167">allowScreenCapture</span></span>|<span data-ttu-id="b2cff-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2cff-168">Boolean</span></span>|<span data-ttu-id="b2cff-169">Indica se a capacidade de captura de tela deve ou não ser permitida durante um teste.</span><span class="sxs-lookup"><span data-stu-id="b2cff-169">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="b2cff-170">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="b2cff-170">allowTextSuggestion</span></span>|<span data-ttu-id="b2cff-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2cff-171">Boolean</span></span>|<span data-ttu-id="b2cff-172">Indica se sugestões de texto devem ou não ser permitidas durante o teste.</span><span class="sxs-lookup"><span data-stu-id="b2cff-172">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="b2cff-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2cff-173">Response</span></span>
<span data-ttu-id="b2cff-174">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2cff-174">If successful, this method returns a `200 OK` response code and an updated [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2cff-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2cff-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2cff-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2cff-176">Request</span></span>
<span data-ttu-id="b2cff-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2cff-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b2cff-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2cff-178">Response</span></span>
<span data-ttu-id="b2cff-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b2cff-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









