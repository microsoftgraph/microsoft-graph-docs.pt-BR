---
title: Criar windows10SecureAssessmentConfiguration
description: Cria um novo objeto windows10SecureAssessmentConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d19b2659e58c71a95266e2cda9209b7ccfac50a5
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760479"
---
# <a name="create-windows10secureassessmentconfiguration"></a><span data-ttu-id="4bc49-103">Criar windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="4bc49-103">Create windows10SecureAssessmentConfiguration</span></span>

<span data-ttu-id="4bc49-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4bc49-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4bc49-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4bc49-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4bc49-106">Cria um novo objeto [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4bc49-106">Create a new [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4bc49-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4bc49-107">Prerequisites</span></span>
<span data-ttu-id="4bc49-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bc49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bc49-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4bc49-110">Permission type</span></span>|<span data-ttu-id="4bc49-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4bc49-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4bc49-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4bc49-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4bc49-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bc49-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4bc49-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4bc49-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4bc49-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4bc49-115">Not supported.</span></span>|
|<span data-ttu-id="4bc49-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4bc49-116">Application</span></span>|<span data-ttu-id="4bc49-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bc49-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4bc49-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4bc49-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4bc49-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4bc49-119">Request headers</span></span>
|<span data-ttu-id="4bc49-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4bc49-120">Header</span></span>|<span data-ttu-id="4bc49-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4bc49-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4bc49-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4bc49-122">Authorization</span></span>|<span data-ttu-id="4bc49-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4bc49-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4bc49-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4bc49-124">Accept</span></span>|<span data-ttu-id="4bc49-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4bc49-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bc49-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4bc49-126">Request body</span></span>
<span data-ttu-id="4bc49-127">No corpo da solicitação, forneça uma representação JSON do objeto windows10SecureAssessmentConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4bc49-127">In the request body, supply a JSON representation for the windows10SecureAssessmentConfiguration object.</span></span>

<span data-ttu-id="4bc49-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10SecureAssessmentConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4bc49-128">The following table shows the properties that are required when you create the windows10SecureAssessmentConfiguration.</span></span>

|<span data-ttu-id="4bc49-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4bc49-129">Property</span></span>|<span data-ttu-id="4bc49-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4bc49-130">Type</span></span>|<span data-ttu-id="4bc49-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4bc49-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bc49-132">id</span><span class="sxs-lookup"><span data-stu-id="4bc49-132">id</span></span>|<span data-ttu-id="4bc49-133">String</span><span class="sxs-lookup"><span data-stu-id="4bc49-133">String</span></span>|<span data-ttu-id="4bc49-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4bc49-134">Key of the entity.</span></span> <span data-ttu-id="4bc49-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4bc49-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4bc49-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4bc49-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4bc49-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4bc49-137">DateTimeOffset</span></span>|<span data-ttu-id="4bc49-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="4bc49-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4bc49-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4bc49-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4bc49-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4bc49-140">createdDateTime</span></span>|<span data-ttu-id="4bc49-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4bc49-141">DateTimeOffset</span></span>|<span data-ttu-id="4bc49-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="4bc49-142">DateTime the object was created.</span></span> <span data-ttu-id="4bc49-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4bc49-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4bc49-144">description</span><span class="sxs-lookup"><span data-stu-id="4bc49-144">description</span></span>|<span data-ttu-id="4bc49-145">String</span><span class="sxs-lookup"><span data-stu-id="4bc49-145">String</span></span>|<span data-ttu-id="4bc49-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4bc49-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4bc49-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4bc49-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4bc49-148">displayName</span><span class="sxs-lookup"><span data-stu-id="4bc49-148">displayName</span></span>|<span data-ttu-id="4bc49-149">String</span><span class="sxs-lookup"><span data-stu-id="4bc49-149">String</span></span>|<span data-ttu-id="4bc49-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4bc49-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4bc49-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4bc49-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4bc49-152">versão</span><span class="sxs-lookup"><span data-stu-id="4bc49-152">version</span></span>|<span data-ttu-id="4bc49-153">Int32</span><span class="sxs-lookup"><span data-stu-id="4bc49-153">Int32</span></span>|<span data-ttu-id="4bc49-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4bc49-154">Version of the device configuration.</span></span> <span data-ttu-id="4bc49-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4bc49-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4bc49-156">launchUri</span><span class="sxs-lookup"><span data-stu-id="4bc49-156">launchUri</span></span>|<span data-ttu-id="4bc49-157">String</span><span class="sxs-lookup"><span data-stu-id="4bc49-157">String</span></span>|<span data-ttu-id="4bc49-158">Link de URL para uma avaliação que é carregada automaticamente quando o navegador de avaliação segura é iniciado.</span><span class="sxs-lookup"><span data-stu-id="4bc49-158">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="4bc49-159">Ele precisa ser um URL válido (http\[s\]://msdn.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="4bc49-159">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="4bc49-160">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="4bc49-160">configurationAccount</span></span>|<span data-ttu-id="4bc49-161">String</span><span class="sxs-lookup"><span data-stu-id="4bc49-161">String</span></span>|<span data-ttu-id="4bc49-162">A conta usada para configurar o dispositivo Windows para realizar o teste.</span><span class="sxs-lookup"><span data-stu-id="4bc49-162">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="4bc49-163">O usuário pode ser uma conta de domínio (domínio\usuário), uma conta do AAD (nomedeusuário@locatário.com) ou uma conta local (nomedeusuário).</span><span class="sxs-lookup"><span data-stu-id="4bc49-163">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="4bc49-164">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="4bc49-164">allowPrinting</span></span>|<span data-ttu-id="4bc49-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="4bc49-165">Boolean</span></span>|<span data-ttu-id="4bc49-166">Indica se o aplicativo deve ou não ter permissão de impressão durante o teste.</span><span class="sxs-lookup"><span data-stu-id="4bc49-166">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="4bc49-167">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="4bc49-167">allowScreenCapture</span></span>|<span data-ttu-id="4bc49-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="4bc49-168">Boolean</span></span>|<span data-ttu-id="4bc49-169">Indica se a capacidade de captura de tela deve ou não ser permitida durante um teste.</span><span class="sxs-lookup"><span data-stu-id="4bc49-169">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="4bc49-170">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="4bc49-170">allowTextSuggestion</span></span>|<span data-ttu-id="4bc49-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="4bc49-171">Boolean</span></span>|<span data-ttu-id="4bc49-172">Indica se sugestões de texto devem ou não ser permitidas durante o teste.</span><span class="sxs-lookup"><span data-stu-id="4bc49-172">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="4bc49-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bc49-173">Response</span></span>
<span data-ttu-id="4bc49-174">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4bc49-174">If successful, this method returns a `201 Created` response code and a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bc49-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4bc49-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="4bc49-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4bc49-176">Request</span></span>
<span data-ttu-id="4bc49-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4bc49-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="4bc49-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bc49-178">Response</span></span>
<span data-ttu-id="4bc49-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4bc49-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




