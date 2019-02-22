---
title: Atualizar windows10SecureAssessmentConfiguration
description: Atualizar as propriedades de um objeto windows10SecureAssessmentConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ab526fee376dbe2c332f8233200e7576b4bf74b1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167820"
---
# <a name="update-windows10secureassessmentconfiguration"></a><span data-ttu-id="77661-103">Atualizar windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="77661-103">Update windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="77661-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="77661-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77661-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="77661-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77661-106">Atualizar as propriedades de um objeto [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77661-106">Update the properties of a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77661-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="77661-107">Prerequisites</span></span>
<span data-ttu-id="77661-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="77661-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="77661-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77661-110">Permission type</span></span>|<span data-ttu-id="77661-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="77661-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77661-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77661-112">Delegated (work or school account)</span></span>|<span data-ttu-id="77661-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77661-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="77661-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77661-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77661-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77661-115">Not supported.</span></span>|
|<span data-ttu-id="77661-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77661-116">Application</span></span>|<span data-ttu-id="77661-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77661-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77661-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77661-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="77661-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77661-119">Request headers</span></span>
|<span data-ttu-id="77661-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="77661-120">Header</span></span>|<span data-ttu-id="77661-121">Valor</span><span class="sxs-lookup"><span data-stu-id="77661-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77661-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="77661-122">Authorization</span></span>|<span data-ttu-id="77661-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77661-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77661-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="77661-124">Accept</span></span>|<span data-ttu-id="77661-125">application/json</span><span class="sxs-lookup"><span data-stu-id="77661-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77661-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77661-126">Request body</span></span>
<span data-ttu-id="77661-127">No corpo da solicitação, forneça uma representação JSON do objeto [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77661-127">In the request body, supply a JSON representation for the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

<span data-ttu-id="77661-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77661-128">The following table shows the properties that are required when you create the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span></span>

|<span data-ttu-id="77661-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="77661-129">Property</span></span>|<span data-ttu-id="77661-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="77661-130">Type</span></span>|<span data-ttu-id="77661-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="77661-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77661-132">id</span><span class="sxs-lookup"><span data-stu-id="77661-132">id</span></span>|<span data-ttu-id="77661-133">String</span><span class="sxs-lookup"><span data-stu-id="77661-133">String</span></span>|<span data-ttu-id="77661-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="77661-134">Key of the entity.</span></span> <span data-ttu-id="77661-135">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77661-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77661-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="77661-136">lastModifiedDateTime</span></span>|<span data-ttu-id="77661-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77661-137">DateTimeOffset</span></span>|<span data-ttu-id="77661-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="77661-138">DateTime the object was last modified.</span></span> <span data-ttu-id="77661-139">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77661-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77661-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="77661-140">roleScopeTagIds</span></span>|<span data-ttu-id="77661-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="77661-141">String collection</span></span>|<span data-ttu-id="77661-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="77661-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="77661-143">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77661-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77661-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="77661-144">supportsScopeTags</span></span>|<span data-ttu-id="77661-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="77661-145">Boolean</span></span>|<span data-ttu-id="77661-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="77661-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="77661-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="77661-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="77661-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="77661-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="77661-149">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="77661-149">This property is read-only.</span></span> <span data-ttu-id="77661-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77661-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77661-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="77661-151">createdDateTime</span></span>|<span data-ttu-id="77661-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77661-152">DateTimeOffset</span></span>|<span data-ttu-id="77661-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="77661-153">DateTime the object was created.</span></span> <span data-ttu-id="77661-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77661-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77661-155">description</span><span class="sxs-lookup"><span data-stu-id="77661-155">description</span></span>|<span data-ttu-id="77661-156">String</span><span class="sxs-lookup"><span data-stu-id="77661-156">String</span></span>|<span data-ttu-id="77661-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="77661-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="77661-158">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77661-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77661-159">displayName</span><span class="sxs-lookup"><span data-stu-id="77661-159">displayName</span></span>|<span data-ttu-id="77661-160">String</span><span class="sxs-lookup"><span data-stu-id="77661-160">String</span></span>|<span data-ttu-id="77661-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="77661-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="77661-162">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77661-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77661-163">version</span><span class="sxs-lookup"><span data-stu-id="77661-163">version</span></span>|<span data-ttu-id="77661-164">Int32</span><span class="sxs-lookup"><span data-stu-id="77661-164">Int32</span></span>|<span data-ttu-id="77661-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="77661-165">Version of the device configuration.</span></span> <span data-ttu-id="77661-166">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77661-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77661-167">launchUri</span><span class="sxs-lookup"><span data-stu-id="77661-167">launchUri</span></span>|<span data-ttu-id="77661-168">String</span><span class="sxs-lookup"><span data-stu-id="77661-168">String</span></span>|<span data-ttu-id="77661-169">Link da URL para uma avaliação que é carregada automaticamente quando o navegador de avaliação segura é iniciado.</span><span class="sxs-lookup"><span data-stu-id="77661-169">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="77661-170">Ele precisa ser uma URL válida (http\[s\]://msdn.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="77661-170">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="77661-171">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="77661-171">configurationAccount</span></span>|<span data-ttu-id="77661-172">String</span><span class="sxs-lookup"><span data-stu-id="77661-172">String</span></span>|<span data-ttu-id="77661-173">A conta usada para configurar o dispositivo Windows para realizar o teste.</span><span class="sxs-lookup"><span data-stu-id="77661-173">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="77661-174">O usuário pode ser uma conta de domínio (domínio\usuário), uma conta do AAD (nomedeusuário@locatário.com) ou uma conta local (nomedeusuário).</span><span class="sxs-lookup"><span data-stu-id="77661-174">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="77661-175">configurationAccountType</span><span class="sxs-lookup"><span data-stu-id="77661-175">configurationAccountType</span></span>|[<span data-ttu-id="77661-176">secureAssessmentAccountType</span><span class="sxs-lookup"><span data-stu-id="77661-176">secureAssessmentAccountType</span></span>](../resources/intune-deviceconfig-secureassessmentaccounttype.md)|<span data-ttu-id="77661-177">O tipo de conta usado pelo ConfigurationAccount.</span><span class="sxs-lookup"><span data-stu-id="77661-177">The account type used to by ConfigurationAccount.</span></span> <span data-ttu-id="77661-178">Os valores possíveis são: `azureADAccount`, `domainAccount`, `localAccount`.</span><span class="sxs-lookup"><span data-stu-id="77661-178">Possible values are: `azureADAccount`, `domainAccount`, `localAccount`.</span></span>|
|<span data-ttu-id="77661-179">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="77661-179">allowPrinting</span></span>|<span data-ttu-id="77661-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="77661-180">Boolean</span></span>|<span data-ttu-id="77661-181">Indica se o aplicativo deve ou não ter permissão de impressão durante o teste.</span><span class="sxs-lookup"><span data-stu-id="77661-181">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="77661-182">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="77661-182">allowScreenCapture</span></span>|<span data-ttu-id="77661-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="77661-183">Boolean</span></span>|<span data-ttu-id="77661-184">Indica se a capacidade de captura de tela deve ou não ser permitida durante um teste.</span><span class="sxs-lookup"><span data-stu-id="77661-184">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="77661-185">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="77661-185">allowTextSuggestion</span></span>|<span data-ttu-id="77661-186">Booliano</span><span class="sxs-lookup"><span data-stu-id="77661-186">Boolean</span></span>|<span data-ttu-id="77661-187">Indica se sugestões de texto devem ou não ser permitidas durante o teste.</span><span class="sxs-lookup"><span data-stu-id="77661-187">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="77661-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="77661-188">Response</span></span>
<span data-ttu-id="77661-189">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77661-189">If successful, this method returns a `200 OK` response code and an updated [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77661-190">Exemplo</span><span class="sxs-lookup"><span data-stu-id="77661-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="77661-191">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77661-191">Request</span></span>
<span data-ttu-id="77661-192">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="77661-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 499

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "configurationAccountType": "domainAccount",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```

### <a name="response"></a><span data-ttu-id="77661-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="77661-193">Response</span></span>
<span data-ttu-id="77661-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="77661-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 671

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "id": "f60d71be-71be-f60d-be71-0df6be710df6",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "configurationAccountType": "domainAccount",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```




