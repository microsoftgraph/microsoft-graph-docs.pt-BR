---
title: Criar windows10XVpnConfiguration
description: Crie um novo objeto windows10XVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f80bb41a3098931af7b10521dce9b803911a474a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145058"
---
# <a name="create-windows10xvpnconfiguration"></a><span data-ttu-id="6e51c-103">Criar windows10XVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="6e51c-103">Create windows10XVpnConfiguration</span></span>

<span data-ttu-id="6e51c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e51c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6e51c-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6e51c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e51c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6e51c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e51c-107">Crie um novo [objeto windows10XVpnConfiguration.](../resources/intune-rapolicy-windows10xvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e51c-107">Create a new [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e51c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6e51c-108">Prerequisites</span></span>
<span data-ttu-id="6e51c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e51c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e51c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e51c-111">Permission type</span></span>|<span data-ttu-id="6e51c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6e51c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e51c-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e51c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6e51c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e51c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6e51c-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e51c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e51c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e51c-116">Not supported.</span></span>|
|<span data-ttu-id="6e51c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e51c-117">Application</span></span>|<span data-ttu-id="6e51c-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e51c-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e51c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e51c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceAccessProfiles
```

## <a name="request-headers"></a><span data-ttu-id="6e51c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e51c-120">Request headers</span></span>
|<span data-ttu-id="6e51c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6e51c-121">Header</span></span>|<span data-ttu-id="6e51c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6e51c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e51c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e51c-123">Authorization</span></span>|<span data-ttu-id="6e51c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e51c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e51c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6e51c-125">Accept</span></span>|<span data-ttu-id="6e51c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6e51c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e51c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e51c-127">Request body</span></span>
<span data-ttu-id="6e51c-128">No corpo da solicitação, fornece uma representação JSON para o objeto windows10XVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6e51c-128">In the request body, supply a JSON representation for the windows10XVpnConfiguration object.</span></span>

<span data-ttu-id="6e51c-129">A tabela a seguir mostra as propriedades necessárias ao criar o windows10XVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6e51c-129">The following table shows the properties that are required when you create the windows10XVpnConfiguration.</span></span>

|<span data-ttu-id="6e51c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e51c-130">Property</span></span>|<span data-ttu-id="6e51c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e51c-131">Type</span></span>|<span data-ttu-id="6e51c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e51c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e51c-133">id</span><span class="sxs-lookup"><span data-stu-id="6e51c-133">id</span></span>|<span data-ttu-id="6e51c-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e51c-134">String</span></span>|<span data-ttu-id="6e51c-135">Identificador de perfil Herdado [de deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6e51c-135">Profile identifier Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="6e51c-136">versão</span><span class="sxs-lookup"><span data-stu-id="6e51c-136">version</span></span>|<span data-ttu-id="6e51c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="6e51c-137">Int32</span></span>|<span data-ttu-id="6e51c-138">Versão do perfil Herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6e51c-138">Version of the profile Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="6e51c-139">displayName</span><span class="sxs-lookup"><span data-stu-id="6e51c-139">displayName</span></span>|<span data-ttu-id="6e51c-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e51c-140">String</span></span>|<span data-ttu-id="6e51c-141">Nome de exibição de perfil Herdado [de deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6e51c-141">Profile display name Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="6e51c-142">descrição</span><span class="sxs-lookup"><span data-stu-id="6e51c-142">description</span></span>|<span data-ttu-id="6e51c-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e51c-143">String</span></span>|<span data-ttu-id="6e51c-144">Descrição de perfil [Herdada de deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6e51c-144">Profile description Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="6e51c-145">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="6e51c-145">creationDateTime</span></span>|<span data-ttu-id="6e51c-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e51c-146">DateTimeOffset</span></span>|<span data-ttu-id="6e51c-147">Perfil DateTime foi criado Herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6e51c-147">DateTime profile was created Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="6e51c-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6e51c-148">lastModifiedDateTime</span></span>|<span data-ttu-id="6e51c-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e51c-149">DateTimeOffset</span></span>|<span data-ttu-id="6e51c-150">O perfil DateTime foi modificado pela última vez Herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6e51c-150">DateTime profile was last modified Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="6e51c-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6e51c-151">roleScopeTagIds</span></span>|<span data-ttu-id="6e51c-152">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e51c-152">String collection</span></span>|<span data-ttu-id="6e51c-153">Marcas de escopo herdadas [de deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6e51c-153">Scope Tags Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="6e51c-154">authenticationCertificateId</span><span class="sxs-lookup"><span data-stu-id="6e51c-154">authenticationCertificateId</span></span>|<span data-ttu-id="6e51c-155">Guid</span><span class="sxs-lookup"><span data-stu-id="6e51c-155">Guid</span></span>|<span data-ttu-id="6e51c-156">ID do Certificado de Autenticação</span><span class="sxs-lookup"><span data-stu-id="6e51c-156">ID to the Authentication Certificate</span></span>|
|<span data-ttu-id="6e51c-157">customXmlFileName</span><span class="sxs-lookup"><span data-stu-id="6e51c-157">customXmlFileName</span></span>|<span data-ttu-id="6e51c-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e51c-158">String</span></span>|<span data-ttu-id="6e51c-159">Nome do arquivo Xml personalizado.</span><span class="sxs-lookup"><span data-stu-id="6e51c-159">Custom Xml file name.</span></span>|
|<span data-ttu-id="6e51c-160">customXml</span><span class="sxs-lookup"><span data-stu-id="6e51c-160">customXml</span></span>|<span data-ttu-id="6e51c-161">Binário</span><span class="sxs-lookup"><span data-stu-id="6e51c-161">Binary</span></span>|<span data-ttu-id="6e51c-162">Comandos XML personalizados que configuram a conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="6e51c-162">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="6e51c-163">(Codificação de byte UTF8)</span><span class="sxs-lookup"><span data-stu-id="6e51c-163">(UTF8 byte encoding)</span></span>|



## <a name="response"></a><span data-ttu-id="6e51c-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e51c-164">Response</span></span>
<span data-ttu-id="6e51c-165">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e51c-165">If successful, this method returns a `201 Created` response code and a [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e51c-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6e51c-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e51c-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e51c-167">Request</span></span>
<span data-ttu-id="6e51c-168">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e51c-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles
Content-type: application/json
Content-length: 446

{
  "@odata.type": "#microsoft.graph.windows10XVpnConfiguration",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "authenticationCertificateId": "39b4cd38-cd38-39b4-38cd-b43938cdb439",
  "customXmlFileName": "Custom Xml File Name value",
  "customXml": "Y3VzdG9tWG1s"
}
```

### <a name="response"></a><span data-ttu-id="6e51c-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e51c-169">Response</span></span>
<span data-ttu-id="6e51c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6e51c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 559

{
  "@odata.type": "#microsoft.graph.windows10XVpnConfiguration",
  "id": "6ee1c04f-c04f-6ee1-4fc0-e16e4fc0e16e",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "authenticationCertificateId": "39b4cd38-cd38-39b4-38cd-b43938cdb439",
  "customXmlFileName": "Custom Xml File Name value",
  "customXml": "Y3VzdG9tWG1s"
}
```




