---
title: Atualizar windows10XVpnConfiguration
description: Atualiza as propriedades de um objeto windows10XVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 38ba34537432f253a530f8c65ca2bd3e4f5f2192
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301372"
---
# <a name="update-windows10xvpnconfiguration"></a><span data-ttu-id="e8e72-103">Atualizar windows10XVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="e8e72-103">Update windows10XVpnConfiguration</span></span>

<span data-ttu-id="e8e72-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8e72-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e8e72-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e8e72-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8e72-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e8e72-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8e72-107">Atualiza as propriedades de um objeto [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e8e72-107">Update the properties of a [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8e72-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e8e72-108">Prerequisites</span></span>
<span data-ttu-id="e8e72-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8e72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8e72-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8e72-111">Permission type</span></span>|<span data-ttu-id="e8e72-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e8e72-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8e72-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8e72-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e8e72-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8e72-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e8e72-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8e72-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8e72-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8e72-116">Not supported.</span></span>|
|<span data-ttu-id="e8e72-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8e72-117">Application</span></span>|<span data-ttu-id="e8e72-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8e72-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8e72-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8e72-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}
```

## <a name="request-headers"></a><span data-ttu-id="e8e72-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8e72-120">Request headers</span></span>
|<span data-ttu-id="e8e72-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e8e72-121">Header</span></span>|<span data-ttu-id="e8e72-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e8e72-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8e72-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8e72-123">Authorization</span></span>|<span data-ttu-id="e8e72-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8e72-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8e72-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e8e72-125">Accept</span></span>|<span data-ttu-id="e8e72-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e8e72-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8e72-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8e72-127">Request body</span></span>
<span data-ttu-id="e8e72-128">No corpo da solicitação, forneça uma representação JSON do objeto [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e8e72-128">In the request body, supply a JSON representation for the [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md) object.</span></span>

<span data-ttu-id="e8e72-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e8e72-129">The following table shows the properties that are required when you create the [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md).</span></span>

|<span data-ttu-id="e8e72-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8e72-130">Property</span></span>|<span data-ttu-id="e8e72-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8e72-131">Type</span></span>|<span data-ttu-id="e8e72-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8e72-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8e72-133">id</span><span class="sxs-lookup"><span data-stu-id="e8e72-133">id</span></span>|<span data-ttu-id="e8e72-134">String</span><span class="sxs-lookup"><span data-stu-id="e8e72-134">String</span></span>|<span data-ttu-id="e8e72-135">Identificador de perfil herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="e8e72-135">Profile identifier Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="e8e72-136">versão</span><span class="sxs-lookup"><span data-stu-id="e8e72-136">version</span></span>|<span data-ttu-id="e8e72-137">Int32</span><span class="sxs-lookup"><span data-stu-id="e8e72-137">Int32</span></span>|<span data-ttu-id="e8e72-138">Versão do perfil herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="e8e72-138">Version of the profile Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="e8e72-139">displayName</span><span class="sxs-lookup"><span data-stu-id="e8e72-139">displayName</span></span>|<span data-ttu-id="e8e72-140">String</span><span class="sxs-lookup"><span data-stu-id="e8e72-140">String</span></span>|<span data-ttu-id="e8e72-141">Nome de exibição do perfil herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="e8e72-141">Profile display name Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="e8e72-142">description</span><span class="sxs-lookup"><span data-stu-id="e8e72-142">description</span></span>|<span data-ttu-id="e8e72-143">String</span><span class="sxs-lookup"><span data-stu-id="e8e72-143">String</span></span>|<span data-ttu-id="e8e72-144">Descrição do perfil herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="e8e72-144">Profile description Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="e8e72-145">creationDatetime</span><span class="sxs-lookup"><span data-stu-id="e8e72-145">creationDateTime</span></span>|<span data-ttu-id="e8e72-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8e72-146">DateTimeOffset</span></span>|<span data-ttu-id="e8e72-147">O perfil DateTime foi criado herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="e8e72-147">DateTime profile was created Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="e8e72-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8e72-148">lastModifiedDateTime</span></span>|<span data-ttu-id="e8e72-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8e72-149">DateTimeOffset</span></span>|<span data-ttu-id="e8e72-150">O perfil DateTime foi modificado pela última vez de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="e8e72-150">DateTime profile was last modified Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="e8e72-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e8e72-151">roleScopeTagIds</span></span>|<span data-ttu-id="e8e72-152">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e8e72-152">String collection</span></span>|<span data-ttu-id="e8e72-153">Marcas de escopo herdadas de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="e8e72-153">Scope Tags Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="e8e72-154">authenticationCertificateId</span><span class="sxs-lookup"><span data-stu-id="e8e72-154">authenticationCertificateId</span></span>|<span data-ttu-id="e8e72-155">Guid</span><span class="sxs-lookup"><span data-stu-id="e8e72-155">Guid</span></span>|<span data-ttu-id="e8e72-156">ID para o certificado de autenticação</span><span class="sxs-lookup"><span data-stu-id="e8e72-156">ID to the Authentication Certificate</span></span>|
|<span data-ttu-id="e8e72-157">customXmlFileName</span><span class="sxs-lookup"><span data-stu-id="e8e72-157">customXmlFileName</span></span>|<span data-ttu-id="e8e72-158">String</span><span class="sxs-lookup"><span data-stu-id="e8e72-158">String</span></span>|<span data-ttu-id="e8e72-159">Nome de arquivo XML personalizado.</span><span class="sxs-lookup"><span data-stu-id="e8e72-159">Custom Xml file name.</span></span>|
|<span data-ttu-id="e8e72-160">customXml</span><span class="sxs-lookup"><span data-stu-id="e8e72-160">customXml</span></span>|<span data-ttu-id="e8e72-161">Binária</span><span class="sxs-lookup"><span data-stu-id="e8e72-161">Binary</span></span>|<span data-ttu-id="e8e72-162">Comandos XML personalizados que configura a conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="e8e72-162">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="e8e72-163">(Codificação de bytes UTF8)</span><span class="sxs-lookup"><span data-stu-id="e8e72-163">(UTF8 byte encoding)</span></span>|



## <a name="response"></a><span data-ttu-id="e8e72-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8e72-164">Response</span></span>
<span data-ttu-id="e8e72-165">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8e72-165">If successful, this method returns a `200 OK` response code and an updated [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8e72-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8e72-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8e72-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8e72-167">Request</span></span>
<span data-ttu-id="e8e72-168">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8e72-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}
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

### <a name="response"></a><span data-ttu-id="e8e72-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8e72-169">Response</span></span>
<span data-ttu-id="e8e72-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8e72-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




