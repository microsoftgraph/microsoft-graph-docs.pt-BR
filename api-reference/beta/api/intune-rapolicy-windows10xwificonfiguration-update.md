---
title: Atualizar windows10XWifiConfiguration
description: Atualize as propriedades de um objeto windows10XWifiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7cad07060a21968db7877128e5215e45cf07059c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158567"
---
# <a name="update-windows10xwificonfiguration"></a><span data-ttu-id="ebfe7-103">Atualizar windows10XWifiConfiguration</span><span class="sxs-lookup"><span data-stu-id="ebfe7-103">Update windows10XWifiConfiguration</span></span>

<span data-ttu-id="ebfe7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebfe7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ebfe7-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ebfe7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebfe7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ebfe7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebfe7-107">Atualize as propriedades de um [objeto windows10XWifiConfiguration.](../resources/intune-rapolicy-windows10xwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ebfe7-107">Update the properties of a [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ebfe7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ebfe7-108">Prerequisites</span></span>
<span data-ttu-id="ebfe7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebfe7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebfe7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ebfe7-111">Permission type</span></span>|<span data-ttu-id="ebfe7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ebfe7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebfe7-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ebfe7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ebfe7-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebfe7-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ebfe7-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ebfe7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebfe7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ebfe7-116">Not supported.</span></span>|
|<span data-ttu-id="ebfe7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ebfe7-117">Application</span></span>|<span data-ttu-id="ebfe7-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebfe7-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebfe7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ebfe7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}
```

## <a name="request-headers"></a><span data-ttu-id="ebfe7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ebfe7-120">Request headers</span></span>
|<span data-ttu-id="ebfe7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ebfe7-121">Header</span></span>|<span data-ttu-id="ebfe7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ebfe7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ebfe7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ebfe7-123">Authorization</span></span>|<span data-ttu-id="ebfe7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ebfe7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ebfe7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ebfe7-125">Accept</span></span>|<span data-ttu-id="ebfe7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ebfe7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebfe7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ebfe7-127">Request body</span></span>
<span data-ttu-id="ebfe7-128">No corpo da solicitação, fornece uma representação JSON para o [objeto windows10XWifiConfiguration.](../resources/intune-rapolicy-windows10xwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ebfe7-128">In the request body, supply a JSON representation for the [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md) object.</span></span>

<span data-ttu-id="ebfe7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ebfe7-129">The following table shows the properties that are required when you create the [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md).</span></span>

|<span data-ttu-id="ebfe7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ebfe7-130">Property</span></span>|<span data-ttu-id="ebfe7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ebfe7-131">Type</span></span>|<span data-ttu-id="ebfe7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebfe7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebfe7-133">id</span><span class="sxs-lookup"><span data-stu-id="ebfe7-133">id</span></span>|<span data-ttu-id="ebfe7-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ebfe7-134">String</span></span>|<span data-ttu-id="ebfe7-135">Identificador de perfil Herdado [de deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ebfe7-135">Profile identifier Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="ebfe7-136">versão</span><span class="sxs-lookup"><span data-stu-id="ebfe7-136">version</span></span>|<span data-ttu-id="ebfe7-137">Int32</span><span class="sxs-lookup"><span data-stu-id="ebfe7-137">Int32</span></span>|<span data-ttu-id="ebfe7-138">Versão do perfil Herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ebfe7-138">Version of the profile Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="ebfe7-139">displayName</span><span class="sxs-lookup"><span data-stu-id="ebfe7-139">displayName</span></span>|<span data-ttu-id="ebfe7-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ebfe7-140">String</span></span>|<span data-ttu-id="ebfe7-141">Nome de exibição de perfil Herdado [de deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ebfe7-141">Profile display name Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="ebfe7-142">descrição</span><span class="sxs-lookup"><span data-stu-id="ebfe7-142">description</span></span>|<span data-ttu-id="ebfe7-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ebfe7-143">String</span></span>|<span data-ttu-id="ebfe7-144">Descrição de perfil [Herdada de deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ebfe7-144">Profile description Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="ebfe7-145">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="ebfe7-145">creationDateTime</span></span>|<span data-ttu-id="ebfe7-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebfe7-146">DateTimeOffset</span></span>|<span data-ttu-id="ebfe7-147">Perfil DateTime foi criado Herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ebfe7-147">DateTime profile was created Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="ebfe7-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ebfe7-148">lastModifiedDateTime</span></span>|<span data-ttu-id="ebfe7-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebfe7-149">DateTimeOffset</span></span>|<span data-ttu-id="ebfe7-150">O perfil DateTime foi modificado pela última vez Herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ebfe7-150">DateTime profile was last modified Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="ebfe7-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ebfe7-151">roleScopeTagIds</span></span>|<span data-ttu-id="ebfe7-152">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ebfe7-152">String collection</span></span>|<span data-ttu-id="ebfe7-153">Marcas de escopo herdadas [de deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ebfe7-153">Scope Tags Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="ebfe7-154">authenticationCertificateId</span><span class="sxs-lookup"><span data-stu-id="ebfe7-154">authenticationCertificateId</span></span>|<span data-ttu-id="ebfe7-155">Guid</span><span class="sxs-lookup"><span data-stu-id="ebfe7-155">Guid</span></span>|<span data-ttu-id="ebfe7-156">ID do Certificado de Autenticação</span><span class="sxs-lookup"><span data-stu-id="ebfe7-156">ID to the Authentication Certificate</span></span>|
|<span data-ttu-id="ebfe7-157">customXmlFileName</span><span class="sxs-lookup"><span data-stu-id="ebfe7-157">customXmlFileName</span></span>|<span data-ttu-id="ebfe7-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ebfe7-158">String</span></span>|<span data-ttu-id="ebfe7-159">Nome do arquivo Xml personalizado.</span><span class="sxs-lookup"><span data-stu-id="ebfe7-159">Custom Xml file name.</span></span>|
|<span data-ttu-id="ebfe7-160">customXml</span><span class="sxs-lookup"><span data-stu-id="ebfe7-160">customXml</span></span>|<span data-ttu-id="ebfe7-161">Binário</span><span class="sxs-lookup"><span data-stu-id="ebfe7-161">Binary</span></span>|<span data-ttu-id="ebfe7-162">Comandos XML personalizados que configuram a conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="ebfe7-162">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="ebfe7-163">(Codificação de byte UTF8)</span><span class="sxs-lookup"><span data-stu-id="ebfe7-163">(UTF8 byte encoding)</span></span>|



## <a name="response"></a><span data-ttu-id="ebfe7-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebfe7-164">Response</span></span>
<span data-ttu-id="ebfe7-165">Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ebfe7-165">If successful, this method returns a `200 OK` response code and an updated [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebfe7-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ebfe7-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="ebfe7-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ebfe7-167">Request</span></span>
<span data-ttu-id="ebfe7-168">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ebfe7-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}
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

### <a name="response"></a><span data-ttu-id="ebfe7-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebfe7-169">Response</span></span>
<span data-ttu-id="ebfe7-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ebfe7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




