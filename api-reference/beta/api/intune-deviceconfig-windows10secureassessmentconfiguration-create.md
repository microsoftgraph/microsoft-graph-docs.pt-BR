---
title: Criar windows10SecureAssessmentConfiguration
description: Cria um novo objeto windows10SecureAssessmentConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: de072f8c9d62b2dd5f3f4a0c74c49316d6ad0d89
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836579"
---
# <a name="create-windows10secureassessmentconfiguration"></a><span data-ttu-id="c63b7-103">Criar windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="c63b7-103">Create windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="c63b7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c63b7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c63b7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c63b7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c63b7-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c63b7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c63b7-107">Cria um novo objeto [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c63b7-107">Create a new [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c63b7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c63b7-108">Prerequisites</span></span>
<span data-ttu-id="c63b7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c63b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c63b7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c63b7-111">Permission type</span></span>|<span data-ttu-id="c63b7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c63b7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c63b7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c63b7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c63b7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c63b7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c63b7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c63b7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c63b7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c63b7-116">Not supported.</span></span>|
|<span data-ttu-id="c63b7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c63b7-117">Application</span></span>|<span data-ttu-id="c63b7-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c63b7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c63b7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c63b7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c63b7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c63b7-120">Request headers</span></span>
|<span data-ttu-id="c63b7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c63b7-121">Header</span></span>|<span data-ttu-id="c63b7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c63b7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c63b7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c63b7-123">Authorization</span></span>|<span data-ttu-id="c63b7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c63b7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c63b7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c63b7-125">Accept</span></span>|<span data-ttu-id="c63b7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c63b7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c63b7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c63b7-127">Request body</span></span>
<span data-ttu-id="c63b7-128">No corpo da solicitação, forneça uma representação JSON do objeto windows10SecureAssessmentConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c63b7-128">In the request body, supply a JSON representation for the windows10SecureAssessmentConfiguration object.</span></span>

<span data-ttu-id="c63b7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10SecureAssessmentConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c63b7-129">The following table shows the properties that are required when you create the windows10SecureAssessmentConfiguration.</span></span>

|<span data-ttu-id="c63b7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c63b7-130">Property</span></span>|<span data-ttu-id="c63b7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c63b7-131">Type</span></span>|<span data-ttu-id="c63b7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c63b7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c63b7-133">id</span><span class="sxs-lookup"><span data-stu-id="c63b7-133">id</span></span>|<span data-ttu-id="c63b7-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c63b7-134">String</span></span>|<span data-ttu-id="c63b7-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c63b7-135">Key of the entity.</span></span> <span data-ttu-id="c63b7-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c63b7-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c63b7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c63b7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c63b7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c63b7-138">DateTimeOffset</span></span>|<span data-ttu-id="c63b7-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="c63b7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c63b7-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c63b7-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c63b7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c63b7-141">roleScopeTagIds</span></span>|<span data-ttu-id="c63b7-142">String collection</span><span class="sxs-lookup"><span data-stu-id="c63b7-142">String collection</span></span>|<span data-ttu-id="c63b7-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="c63b7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c63b7-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c63b7-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c63b7-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c63b7-145">supportsScopeTags</span></span>|<span data-ttu-id="c63b7-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="c63b7-146">Boolean</span></span>|<span data-ttu-id="c63b7-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="c63b7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c63b7-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="c63b7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c63b7-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="c63b7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c63b7-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c63b7-150">This property is read-only.</span></span> <span data-ttu-id="c63b7-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c63b7-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c63b7-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c63b7-152">createdDateTime</span></span>|<span data-ttu-id="c63b7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c63b7-153">DateTimeOffset</span></span>|<span data-ttu-id="c63b7-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="c63b7-154">DateTime the object was created.</span></span> <span data-ttu-id="c63b7-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c63b7-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c63b7-156">description</span><span class="sxs-lookup"><span data-stu-id="c63b7-156">description</span></span>|<span data-ttu-id="c63b7-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c63b7-157">String</span></span>|<span data-ttu-id="c63b7-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c63b7-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c63b7-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c63b7-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c63b7-160">displayName</span><span class="sxs-lookup"><span data-stu-id="c63b7-160">displayName</span></span>|<span data-ttu-id="c63b7-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c63b7-161">String</span></span>|<span data-ttu-id="c63b7-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c63b7-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c63b7-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c63b7-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c63b7-164">version</span><span class="sxs-lookup"><span data-stu-id="c63b7-164">version</span></span>|<span data-ttu-id="c63b7-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c63b7-165">Int32</span></span>|<span data-ttu-id="c63b7-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c63b7-166">Version of the device configuration.</span></span> <span data-ttu-id="c63b7-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c63b7-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c63b7-168">launchUri</span><span class="sxs-lookup"><span data-stu-id="c63b7-168">launchUri</span></span>|<span data-ttu-id="c63b7-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c63b7-169">String</span></span>|<span data-ttu-id="c63b7-170">Link da URL para uma avaliação que é carregada automaticamente quando o navegador de avaliação segura é iniciado.</span><span class="sxs-lookup"><span data-stu-id="c63b7-170">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="c63b7-171">Ele precisa ser uma URL válida (http\[s\]://msdn.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="c63b7-171">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="c63b7-172">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="c63b7-172">configurationAccount</span></span>|<span data-ttu-id="c63b7-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c63b7-173">String</span></span>|<span data-ttu-id="c63b7-174">A conta usada para configurar o dispositivo Windows para realizar o teste.</span><span class="sxs-lookup"><span data-stu-id="c63b7-174">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="c63b7-175">O usuário pode ser uma conta de domínio (domínio\usuário), uma conta do AAD (nomedeusuário@locatário.com) ou uma conta local (nomedeusuário).</span><span class="sxs-lookup"><span data-stu-id="c63b7-175">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="c63b7-176">configurationAccountType</span><span class="sxs-lookup"><span data-stu-id="c63b7-176">configurationAccountType</span></span>|[<span data-ttu-id="c63b7-177">secureAssessmentAccountType</span><span class="sxs-lookup"><span data-stu-id="c63b7-177">secureAssessmentAccountType</span></span>](../resources/intune-deviceconfig-secureassessmentaccounttype.md)|<span data-ttu-id="c63b7-178">O tipo de conta usado para por ConfigurationAccount.</span><span class="sxs-lookup"><span data-stu-id="c63b7-178">The account type used to by ConfigurationAccount.</span></span> <span data-ttu-id="c63b7-179">Os valores possíveis são: `azureADAccount`, `domainAccount`, `localAccount`.</span><span class="sxs-lookup"><span data-stu-id="c63b7-179">Possible values are: `azureADAccount`, `domainAccount`, `localAccount`.</span></span>|
|<span data-ttu-id="c63b7-180">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="c63b7-180">allowPrinting</span></span>|<span data-ttu-id="c63b7-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="c63b7-181">Boolean</span></span>|<span data-ttu-id="c63b7-182">Indica se o aplicativo deve ou não ter permissão de impressão durante o teste.</span><span class="sxs-lookup"><span data-stu-id="c63b7-182">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="c63b7-183">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="c63b7-183">allowScreenCapture</span></span>|<span data-ttu-id="c63b7-184">Booliano</span><span class="sxs-lookup"><span data-stu-id="c63b7-184">Boolean</span></span>|<span data-ttu-id="c63b7-185">Indica se a capacidade de captura de tela deve ou não ser permitida durante um teste.</span><span class="sxs-lookup"><span data-stu-id="c63b7-185">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="c63b7-186">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="c63b7-186">allowTextSuggestion</span></span>|<span data-ttu-id="c63b7-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="c63b7-187">Boolean</span></span>|<span data-ttu-id="c63b7-188">Indica se sugestões de texto devem ou não ser permitidas durante o teste.</span><span class="sxs-lookup"><span data-stu-id="c63b7-188">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="c63b7-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="c63b7-189">Response</span></span>
<span data-ttu-id="c63b7-190">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c63b7-190">If successful, this method returns a `201 Created` response code and a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c63b7-191">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c63b7-191">Example</span></span>
### <a name="request"></a><span data-ttu-id="c63b7-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c63b7-192">Request</span></span>
<span data-ttu-id="c63b7-193">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c63b7-193">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 563

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="c63b7-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="c63b7-194">Response</span></span>
<span data-ttu-id="c63b7-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c63b7-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





