---
title: Criar windows10XWifiConfiguration
description: Crie um novo objeto windows10XWifiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 08735db11e3cb1c656f80685917d14fb9b58493c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148524"
---
# <a name="create-windows10xwificonfiguration"></a><span data-ttu-id="79558-103">Criar windows10XWifiConfiguration</span><span class="sxs-lookup"><span data-stu-id="79558-103">Create windows10XWifiConfiguration</span></span>

<span data-ttu-id="79558-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79558-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="79558-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="79558-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79558-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="79558-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79558-107">Crie um novo [objeto windows10XWifiConfiguration.](../resources/intune-rapolicy-windows10xwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79558-107">Create a new [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79558-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="79558-108">Prerequisites</span></span>
<span data-ttu-id="79558-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79558-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79558-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79558-111">Permission type</span></span>|<span data-ttu-id="79558-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="79558-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79558-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79558-113">Delegated (work or school account)</span></span>|<span data-ttu-id="79558-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79558-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="79558-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79558-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79558-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79558-116">Not supported.</span></span>|
|<span data-ttu-id="79558-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79558-117">Application</span></span>|<span data-ttu-id="79558-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79558-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="79558-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79558-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceAccessProfiles
```

## <a name="request-headers"></a><span data-ttu-id="79558-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79558-120">Request headers</span></span>
|<span data-ttu-id="79558-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="79558-121">Header</span></span>|<span data-ttu-id="79558-122">Valor</span><span class="sxs-lookup"><span data-stu-id="79558-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79558-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="79558-123">Authorization</span></span>|<span data-ttu-id="79558-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79558-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79558-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="79558-125">Accept</span></span>|<span data-ttu-id="79558-126">application/json</span><span class="sxs-lookup"><span data-stu-id="79558-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79558-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79558-127">Request body</span></span>
<span data-ttu-id="79558-128">No corpo da solicitação, fornece uma representação JSON para o objeto windows10XWifiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="79558-128">In the request body, supply a JSON representation for the windows10XWifiConfiguration object.</span></span>

<span data-ttu-id="79558-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o windows10XWifiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="79558-129">The following table shows the properties that are required when you create the windows10XWifiConfiguration.</span></span>

|<span data-ttu-id="79558-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79558-130">Property</span></span>|<span data-ttu-id="79558-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="79558-131">Type</span></span>|<span data-ttu-id="79558-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="79558-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79558-133">id</span><span class="sxs-lookup"><span data-stu-id="79558-133">id</span></span>|<span data-ttu-id="79558-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79558-134">String</span></span>|<span data-ttu-id="79558-135">Identificador de perfil Herdado [de deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="79558-135">Profile identifier Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="79558-136">versão</span><span class="sxs-lookup"><span data-stu-id="79558-136">version</span></span>|<span data-ttu-id="79558-137">Int32</span><span class="sxs-lookup"><span data-stu-id="79558-137">Int32</span></span>|<span data-ttu-id="79558-138">Versão do perfil Herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="79558-138">Version of the profile Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="79558-139">displayName</span><span class="sxs-lookup"><span data-stu-id="79558-139">displayName</span></span>|<span data-ttu-id="79558-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79558-140">String</span></span>|<span data-ttu-id="79558-141">Nome de exibição de perfil Herdado [de deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="79558-141">Profile display name Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="79558-142">descrição</span><span class="sxs-lookup"><span data-stu-id="79558-142">description</span></span>|<span data-ttu-id="79558-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79558-143">String</span></span>|<span data-ttu-id="79558-144">Descrição de perfil [Herdada de deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="79558-144">Profile description Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="79558-145">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="79558-145">creationDateTime</span></span>|<span data-ttu-id="79558-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79558-146">DateTimeOffset</span></span>|<span data-ttu-id="79558-147">Perfil DateTime foi criado Herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="79558-147">DateTime profile was created Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="79558-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="79558-148">lastModifiedDateTime</span></span>|<span data-ttu-id="79558-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79558-149">DateTimeOffset</span></span>|<span data-ttu-id="79558-150">O perfil DateTime foi modificado pela última vez Herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="79558-150">DateTime profile was last modified Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="79558-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="79558-151">roleScopeTagIds</span></span>|<span data-ttu-id="79558-152">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="79558-152">String collection</span></span>|<span data-ttu-id="79558-153">Marcas de escopo herdadas [de deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="79558-153">Scope Tags Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="79558-154">authenticationCertificateId</span><span class="sxs-lookup"><span data-stu-id="79558-154">authenticationCertificateId</span></span>|<span data-ttu-id="79558-155">Guid</span><span class="sxs-lookup"><span data-stu-id="79558-155">Guid</span></span>|<span data-ttu-id="79558-156">ID do Certificado de Autenticação</span><span class="sxs-lookup"><span data-stu-id="79558-156">ID to the Authentication Certificate</span></span>|
|<span data-ttu-id="79558-157">customXmlFileName</span><span class="sxs-lookup"><span data-stu-id="79558-157">customXmlFileName</span></span>|<span data-ttu-id="79558-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79558-158">String</span></span>|<span data-ttu-id="79558-159">Nome do arquivo Xml personalizado.</span><span class="sxs-lookup"><span data-stu-id="79558-159">Custom Xml file name.</span></span>|
|<span data-ttu-id="79558-160">customXml</span><span class="sxs-lookup"><span data-stu-id="79558-160">customXml</span></span>|<span data-ttu-id="79558-161">Binário</span><span class="sxs-lookup"><span data-stu-id="79558-161">Binary</span></span>|<span data-ttu-id="79558-162">Comandos XML personalizados que configuram a conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="79558-162">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="79558-163">(Codificação de byte UTF8)</span><span class="sxs-lookup"><span data-stu-id="79558-163">(UTF8 byte encoding)</span></span>|



## <a name="response"></a><span data-ttu-id="79558-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="79558-164">Response</span></span>
<span data-ttu-id="79558-165">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79558-165">If successful, this method returns a `201 Created` response code and a [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79558-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="79558-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="79558-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79558-167">Request</span></span>
<span data-ttu-id="79558-168">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="79558-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles
Content-type: application/json
Content-length: 447

{
  "@odata.type": "#microsoft.graph.windows10XWifiConfiguration",
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

### <a name="response"></a><span data-ttu-id="79558-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="79558-169">Response</span></span>
<span data-ttu-id="79558-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="79558-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 560

{
  "@odata.type": "#microsoft.graph.windows10XWifiConfiguration",
  "id": "31063b86-3b86-3106-863b-0631863b0631",
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




