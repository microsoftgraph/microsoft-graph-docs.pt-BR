---
title: Criar windows10SecureAssessmentConfiguration
description: Cria um novo objeto windows10SecureAssessmentConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2919ce12936e5d7387f857de4e5381196c9b5bb9
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37365261"
---
# <a name="create-windows10secureassessmentconfiguration"></a><span data-ttu-id="c8df6-103">Criar windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="c8df6-103">Create windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="c8df6-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c8df6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8df6-105">Cria um novo objeto [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c8df6-105">Create a new [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8df6-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c8df6-106">Prerequisites</span></span>
<span data-ttu-id="c8df6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8df6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8df6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c8df6-109">Permission type</span></span>|<span data-ttu-id="c8df6-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c8df6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8df6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c8df6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c8df6-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8df6-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c8df6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c8df6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8df6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8df6-114">Not supported.</span></span>|
|<span data-ttu-id="c8df6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8df6-115">Application</span></span>|<span data-ttu-id="c8df6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8df6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8df6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c8df6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c8df6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c8df6-118">Request headers</span></span>
|<span data-ttu-id="c8df6-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c8df6-119">Header</span></span>|<span data-ttu-id="c8df6-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c8df6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8df6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c8df6-121">Authorization</span></span>|<span data-ttu-id="c8df6-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c8df6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8df6-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c8df6-123">Accept</span></span>|<span data-ttu-id="c8df6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c8df6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8df6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c8df6-125">Request body</span></span>
<span data-ttu-id="c8df6-126">No corpo da solicitação, forneça uma representação JSON do objeto windows10SecureAssessmentConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c8df6-126">In the request body, supply a JSON representation for the windows10SecureAssessmentConfiguration object.</span></span>

<span data-ttu-id="c8df6-127">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10SecureAssessmentConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c8df6-127">The following table shows the properties that are required when you create the windows10SecureAssessmentConfiguration.</span></span>

|<span data-ttu-id="c8df6-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c8df6-128">Property</span></span>|<span data-ttu-id="c8df6-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8df6-129">Type</span></span>|<span data-ttu-id="c8df6-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8df6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8df6-131">id</span><span class="sxs-lookup"><span data-stu-id="c8df6-131">id</span></span>|<span data-ttu-id="c8df6-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8df6-132">String</span></span>|<span data-ttu-id="c8df6-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c8df6-133">Key of the entity.</span></span> <span data-ttu-id="c8df6-134">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c8df6-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8df6-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c8df6-135">lastModifiedDateTime</span></span>|<span data-ttu-id="c8df6-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8df6-136">DateTimeOffset</span></span>|<span data-ttu-id="c8df6-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="c8df6-137">DateTime the object was last modified.</span></span> <span data-ttu-id="c8df6-138">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c8df6-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8df6-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c8df6-139">createdDateTime</span></span>|<span data-ttu-id="c8df6-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8df6-140">DateTimeOffset</span></span>|<span data-ttu-id="c8df6-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="c8df6-141">DateTime the object was created.</span></span> <span data-ttu-id="c8df6-142">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c8df6-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8df6-143">descrição</span><span class="sxs-lookup"><span data-stu-id="c8df6-143">description</span></span>|<span data-ttu-id="c8df6-144">String</span><span class="sxs-lookup"><span data-stu-id="c8df6-144">String</span></span>|<span data-ttu-id="c8df6-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c8df6-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c8df6-146">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c8df6-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8df6-147">displayName</span><span class="sxs-lookup"><span data-stu-id="c8df6-147">displayName</span></span>|<span data-ttu-id="c8df6-148">String</span><span class="sxs-lookup"><span data-stu-id="c8df6-148">String</span></span>|<span data-ttu-id="c8df6-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c8df6-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c8df6-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c8df6-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8df6-151">versão</span><span class="sxs-lookup"><span data-stu-id="c8df6-151">version</span></span>|<span data-ttu-id="c8df6-152">Int32</span><span class="sxs-lookup"><span data-stu-id="c8df6-152">Int32</span></span>|<span data-ttu-id="c8df6-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c8df6-153">Version of the device configuration.</span></span> <span data-ttu-id="c8df6-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c8df6-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8df6-155">launchUri</span><span class="sxs-lookup"><span data-stu-id="c8df6-155">launchUri</span></span>|<span data-ttu-id="c8df6-156">String</span><span class="sxs-lookup"><span data-stu-id="c8df6-156">String</span></span>|<span data-ttu-id="c8df6-157">Link de URL para uma avaliação que é carregada automaticamente quando o navegador de avaliação segura é iniciado.</span><span class="sxs-lookup"><span data-stu-id="c8df6-157">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="c8df6-158">Ele precisa ser um URL válido (http\[s\]://msdn.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="c8df6-158">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="c8df6-159">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="c8df6-159">configurationAccount</span></span>|<span data-ttu-id="c8df6-160">String</span><span class="sxs-lookup"><span data-stu-id="c8df6-160">String</span></span>|<span data-ttu-id="c8df6-161">A conta usada para configurar o dispositivo Windows para realizar o teste.</span><span class="sxs-lookup"><span data-stu-id="c8df6-161">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="c8df6-162">O usuário pode ser uma conta de domínio (domínio\usuário), uma conta do AAD (nomedeusuário@locatário.com) ou uma conta local (nomedeusuário).</span><span class="sxs-lookup"><span data-stu-id="c8df6-162">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="c8df6-163">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="c8df6-163">allowPrinting</span></span>|<span data-ttu-id="c8df6-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="c8df6-164">Boolean</span></span>|<span data-ttu-id="c8df6-165">Indica se o aplicativo deve ou não ter permissão de impressão durante o teste.</span><span class="sxs-lookup"><span data-stu-id="c8df6-165">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="c8df6-166">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="c8df6-166">allowScreenCapture</span></span>|<span data-ttu-id="c8df6-167">Booliano</span><span class="sxs-lookup"><span data-stu-id="c8df6-167">Boolean</span></span>|<span data-ttu-id="c8df6-168">Indica se a capacidade de captura de tela deve ou não ser permitida durante um teste.</span><span class="sxs-lookup"><span data-stu-id="c8df6-168">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="c8df6-169">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="c8df6-169">allowTextSuggestion</span></span>|<span data-ttu-id="c8df6-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8df6-170">Boolean</span></span>|<span data-ttu-id="c8df6-171">Indica se sugestões de texto devem ou não ser permitidas durante o teste.</span><span class="sxs-lookup"><span data-stu-id="c8df6-171">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="c8df6-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8df6-172">Response</span></span>
<span data-ttu-id="c8df6-173">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c8df6-173">If successful, this method returns a `201 Created` response code and a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8df6-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c8df6-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8df6-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c8df6-175">Request</span></span>
<span data-ttu-id="c8df6-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c8df6-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c8df6-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8df6-177">Response</span></span>
<span data-ttu-id="c8df6-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c8df6-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




